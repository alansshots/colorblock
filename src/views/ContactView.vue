<template>
  <div class="contact">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Контакти</h1>
      </div>
    </div>

    <!-- Main contact  -->
    
    <div class="contact-main">

        <div class="form">
            <form action="">
                <h2>Свържете се с нас</h2>
                <div class="input-container">
                    <label for="name">Име</label>
                    <input type="text" name="name" placeholder="Въведете вашето име">
                </div>
                <div class="input-container">
                    <label for="email">Имейл</label>
                    <input type="email" name="email" placeholder="Въведете вашия имейл">
                </div>
                <div class="input-container">
                    <label for="message">Съобщение</label>
                    <textarea name="message" cols="40" rows="5" placeholder="Въведете вашето съобщение..."></textarea>
                </div>

                <button class="info-btn">Изпрати</button>

            </form>
        </div>

        <div class="details">
            <div class="details-container">
                <div class="detail-block">
                    <h3>Работно време:</h3>
                    <p>9:00 - 15:00, Пон. до Пет.</p>
                </div>

                <div class="detail-block">
                    <h3>Контакти</h3>
                    <p>alengospodinov@gmail.com</p>
                    <p>+359 889 366 414</p>
                </div>
            </div>
        </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'ContactView'
}
</script>

<style scoped>

.banner {
  height: 125px;
  background: url('../assets/banner.jpg');
  background-size: 1000px;
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

/* .info-btn:hover::after {
    transition: 0.6s;
    content: ' ->';
    color: #000;
} */

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