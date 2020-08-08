<template>
  <div class="Body">
        <div class="columns reverse-columns is-vcentered is-variable is-8">
            <div class="column">
                <h1 class="title has-text-primary is-size-1">Use SEQu-HEALTH for FREE</h1>
                <h2 class="subtitle">The First Step in making your business Health Secure</h2>
                <p class="is-size-5">SEQu-HEALTH is the industry-leading free basic daily health declaration for your employees and guests</p>
                <p class="is-size-7">We are offering SEQu-HEALTH for free to eligible companies. Kindly fill up the form and our Solutions Architects will contact you to get started.</p>
                <form action=" https://formsubmit.co/jpatdu@smpcopartners.com" method="POST">
                    <b-field label="Company Name">
                        <b-input type="text" name="name" required></b-input>
                    </b-field>
                    <b-field label="Email Address">
                        <b-input type="email" name="email" required></b-input>
                    </b-field>
                    <b-field label="Cellphone Number">
                        <b-input type="text" name="PhoneNumber" required></b-input>
                    </b-field>
                    <input type="hidden" name="_subject" value="SEQu-HEALTH Request">
                    <input type="hidden" name="_cc" value="dmanalastas@smpcopartners.com">
                    <input type="hidden" name="_replyto">
                    <input type="text" name="_honey" style="display:none">
                    <b-button tag="button" type="is-primary" native-type="submit">Submit</b-button>
                </form>
            </div>
            <div class="column">
                <img src="img/sequ-health.jpg"/>
            </div>
        </div>
        <div class="box">
            <h1 class="has-text-centered title has-text-primary">Become Health Secure Today</h1>
            <b-button tag="a"
                      href="https://share.hsforms.com/1HFKFFJkKRTSZ_WTIhQVSFw4lq3k"
                      type="is-primary"
                      expanded
                      size="is-medium"
                      target="_blank">
                Download our Brochure
            </b-button>
            <hr>
            <a href="https://sequ-suite.com" target="_blank">
              <h6 class="has-text-centered">
                Learn more about SEQu-SUITE on sequ-suite.com →
              </h6>
            </a>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style scoped>
  .Body {
        padding-left: 10%;
        padding-right: 10%;
        padding-top: 56px;
        padding-bottom: 56px;
    }

  @media(max-width: 767px) {
      .reverse-columns {
          flex-direction: column-reverse;
          display: flex;
      }
  }

  .box {
        padding: 28px;
    }
</style>
