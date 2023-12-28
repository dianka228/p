
<template>
    <footer>
      <div class="footer-content">
        <div class="contact-info">
          <p>Телефон: {{ phoneNumber }}</p>
          <p>Юридический адрес: {{ legalAddress }}</p>
        </div>
        <div class="social-links">
          <a href="ссылка_на_ваш_facebook" target="_blank" rel="noopener noreferrer">Facebook</a>
          <a href="ссылка_на_ваш_twitter" target="_blank" rel="noopener noreferrer">Twitter</a>
          <!-- Добавьте другие социальные сети по аналогии -->
        </div>
      </div>
      <p>&copy; 2023 Ваше название компании. Все права защищены.</p>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer',
    data() {
      return {
        phoneNumber: '+7 (XXX) XXX-XXXX', // Замените на ваш номер телефона
        legalAddress: 'Ваш юридический адрес', // Замените на ваш юридический адрес
      };
    },
  };
  </script>
  
  <style scoped>
  /* Стили для вашего футера */
  footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .contact-info {
    text-align: left;
  }
  
  .social-links a {
    color: #fff;
    margin-right: 10px;
    text-decoration: none;
  }
  
  .social-links a:hover {
    text-decoration: underline;
  }
  </style>