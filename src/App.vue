<template>
  <div class="contact-container">
    <div class="contact-card">
      <!-- Seção do Perfil -->
      <div class="profile-section">
        <div class="profile-image">
          <img src="./assets/profile.png" alt="Foto de Perfil" class="profile-img" />
        </div>
        <h1 class="contact-title">Entre em Contato</h1>
        <p class="contact-subtitle">
          Olá! Fico feliz que você queira entrar em contato. Sinta-se à vontade para me seguir nas redes sociais ou enviar um email.
        </p>
      </div>

      <!-- Links das Redes Sociais -->
      <div class="social-links">
        <a 
          href="https://www.instagram.com/g_france07/" 
          target="_blank" 
          class="social-link instagram tooltip"
          data-tooltip="Instagram"
          @click="handleSocialClick('Instagram')"
        >
          <i class="fab fa-instagram"></i>
        </a>
        
        <a 
          href="https://www.linkedin.com/in/guilherme-france-de-oliveira-santos-9435aa360/" 
          target="_blank" 
          class="social-link linkedin tooltip"
          data-tooltip="LinkedIn"
          @click="handleSocialClick('LinkedIn')"
        >
          <i class="fab fa-linkedin-in"></i>
        </a>
        
        <a 
          href="https://github.com/GuilhermeFrance" 
          target="_blank" 
          class="social-link github tooltip"
          data-tooltip="GitHub"
          @click="handleSocialClick('GitHub')"
        >
          <i class="fab fa-github"></i>
        </a>
        
        <a 
          href="https://wa.me/5577988653938" 
          target="_blank" 
          class="social-link whatsapp tooltip"
          data-tooltip="WhatsApp"
          @click="handleSocialClick('WhatsApp')"
        >
          <i class="fab fa-whatsapp"></i>
        </a>
      </div>

      <!-- Informações de Contato -->
      <div class="contact-info">
        <p class="contact-text">
          Estou sempre aberto a novas oportunidades, colaborações interessantes. Entre em contato:
        </p>
        
        <a 
          href="mailto:guilhermefrance9@gmail.com" 
          class="contact-email"
          @click="handleEmailClick"
        >
          <i class="fas fa-envelope"></i>
          Enviar Email
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactPage',
  methods: {
    handleSocialClick(platform) {
      console.log(`Redirecionando para ${platform}`);
      // Aqui você pode adicionar analytics ou outras funcionalidades
    },
    
    handleEmailClick() {
      console.log('Abrindo cliente de email');
      // Aqui você pode adicionar analytics ou outras funcionalidades
    }
  }
}
</script>