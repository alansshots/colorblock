<template>
  <div class="contact page">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Контакти</h1>
      </div>
    </div>

    <!-- Main contact  -->
    
    <div class="contact-main">

        <div class="form">
            <form  ref="form" @submit.prevent="sendEmail">
                <h2>Свържете се с нас</h2>
                <div class="input-container">
                    <label for="name">Име</label>
                    <input type="text" name="user_name" placeholder="Въведете вашето име">
                </div>
                <div class="input-container">
                    <label for="email">Имейл</label>
                    <input type="email" name="user_email" placeholder="Въведете вашия имейл">
                </div>
                <div class="input-container">
                    <label for="message">Съобщение</label>
                    <textarea name="message" cols="40" rows="5" placeholder="Въведете вашето съобщение..."></textarea>
                </div>

                <button class="info-btn">Изпрати</button>

                <div class="alert-true hidden" role="alert">
                    <span >Вашето запитване беше успешно изпратено!</span>
                </div>

                <div class="alert-false hidden" role="alert">
                    <span >Нещо се обърка. Моля опитайте по-късно.</span>
                </div>
            </form>
        </div>

        <div class="details">
            <div class="details-container">
                <div class="detail-block">
                    <h3>Работно време:</h3>
                    <p>10:00 - 18:00, Пон. до Пет.</p>
                </div>

                <div class="detail-block">
                    <h3>Контакти</h3>
                    <p>hello@colorblockweb.com</p>
                    <p>+359 889 366 414</p>
                </div>
            </div>
        </div>

    </div>

  </div>
</template>

<script>
import emailjs from '@emailjs/browser';

export default {
  name: 'ContactView',
  data() {
    return {
        emailSuccess: null,
    }
  },
  methods: {
    sendEmail() {
      emailjs.sendForm('service_10ux40j', 'template_ya0dape', this.$refs.form, 'tFPkG7-hDXPzH3GAr')
        .then((result) => {
            console.log('SUCCESS!', result.text);
                document.querySelector('.alert-true').classList.remove('hidden')
            setInterval(() => {
                document.querySelector('.alert-true').classList.remove('hidden')
            }, 4000);
        }, (error) => {
            console.log('FAILED...', error.text);
                document.querySelector('.alert-false').classList.remove('hidden')
            setInterval(() => {
                document.querySelector('.alert-false').classList.add('hidden')
            }, 4000);
        });
    }
  }
}
</script>

<style scoped>

.banner {
  height: 425px;
  background: url('../assets/banner.jpg');
  background-size: 1050px;
  object-fit: contain;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.banner-text-container {
  width: 100%;
  height: 100%;
  background: rgb(0, 0, 0, 0.5);
  color: #fff;
  line-height: 0.1rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

/* Main contact */

.contact-main {
    margin: 3rem 0rem;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: left;
    width: 100%;
}

.form {
    border: 1px solid #000;
    display: flex;
    justify-content: center;
    align-items: left;
    width: 50%;
}

form {
    margin: 1rem 2rem;
    width: 100%;
}

form h2 {
    font-weight: 300;
}

.input-container {
    display: flex;
    flex-direction:column;
    justify-content: center;
    align-items: left;
    margin-top: 1rem;
}

.input-container input {
    margin-top: 0.5rem;
    padding: 0.5rem;
}

.input-container textarea {
    margin-top: 0.5rem;
    padding: 0.5rem;
}

.info-btn {
    width: 100%;
    text-align: center;
    margin: 0.5rem auto;
    cursor: pointer;
    padding: 0.5rem 2rem;
    color: #fff;
    background: #000;
    border: 1px solid #fff;
}

.info-btn:hover {
    padding: 0.5rem 2rem;
    color: #000;
    background: #fff;
    border: 1px solid #000;
    transition:  0.2s;
}

.alert-true {
    margin-top: 10px;
    padding: 10px;
    border: 1px solid black;
    background: #F0FDF4;
}

.alert-false {
    margin-top: 10px;
    padding: 10px;
    border: 1px solid black;
    background: #FEF2F2;
}

/* Contact details */

.details {
    width: 20%;
    display: flex;
    flex-direction: row;
    justify-content: start;
    align-items: left;
}

@media only screen and (max-width: 600px) {
    .contact-main {
        margin-top: 1.5rem;
        flex-direction: column-reverse;
        align-items: center;
    }

    .details {
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }

    .details-container {
        width: 94%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
    }

    .form {
        width: 95%;
        padding: 1rem;
    }

    
}

</style>