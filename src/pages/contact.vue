<template>
  <section id="contact">
    <div class="wrapper">
      <div class="container-fluid">
        <div class="heading">Contact US</div>
        <div class="caption">Come join our network!</div>
        <div class="body mt-5">
          <div class="row mb-5 mt-5">
            <div class="col-lg-1"></div>
            <div class="col-lg-5 text-left">
              <!-- Address -->
              <div class="row m-2 mt-5 mb-3">
                <div class="col-2">
                  <i class="fas fa-map-marked-alt fa-lg"></i>
                </div>
                <div class="address col">
                  <p>5-9-16, 3A, Prashanti Nagar, IDA Kukatpally, Kukatpally, Hyderabad, Telangana 500072</p>
                </div>
              </div>
              <div class="row m-2 mt-3 mb-3">
                <div class="col-2">
                  <a href="mailto:raengineers2444@gmail.com">
                    <i class="far fa-envelope fa-lg"></i>
                  </a>
                </div>
                <div class="email col">
                  <a href="mailto:raengineers2444@gmail.com">raengineers2444@gmail.com</a>
                </div>
              </div>
              <div class="row m-2 mt-5">
                <div class="col-2">
                  <i class="fas fa-phone-alt fa-lg"></i>
                </div>
                <div class="phone col">+91-8919107850</div>
              </div>
            </div>

            <div class="col-lg-4 text-left mt-5 mr-3 align-middle">
              <b-form @submit="onSubmit" v-if="show">
                <b-form-group id="input-group-2" label="Name:" label-for="input-2">
                  <b-form-input
                    id="input-2"
                    v-model="form.name"
                    required
                    placeholder="What's your name?"
                  ></b-form-input>
                </b-form-group>

                <b-form-group id="input-group-2" label="Email:" label-for="input-2">
                  <b-form-input
                    id="input-2"
                    v-model="form.email"
                    type="email"
                    required
                    placeholder="Your E-mail ID?"
                  ></b-form-input>
                </b-form-group>

                <b-form-group id="input-group-2" label="Contact:" label-for="input-number">
                  <b-input-group prepend="+91" class="mb-2 mr-sm-2 mb-sm-0">
                    <b-input
                      v-model="form.number"
                      type="number"
                      id="input-number"
                      placeholder="Need your number, so we can get in touch!"
                    ></b-input>
                  </b-input-group>
                </b-form-group>

                <b-form-group id="input-group-2" label="Message:" label-for="input-2">
                  <b-form-textarea
                    id="input-2"
                    v-model="form.message"
                    type="email"
                    placeholder="Want to say something?"
                    rows="3"
                  ></b-form-textarea>
                </b-form-group>

                <b-form-group id="input-group-4">
                  <b-form-checkbox-group v-model="form.checked" id="checkboxes-4" required>
                    <b-form-checkbox
                      value="true"
                    >I give my consent that anyone from RA Engineers can reach me out</b-form-checkbox>
                  </b-form-checkbox-group>
                </b-form-group>

                <b-button type="submit" variant="primary">Submit</b-button>
              </b-form>
            </div>
            <div class="col-lg-2"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      form: {
        email: "",
        name: "",

        checked: []
      },
      show: true
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      // alert(JSON.stringify(this.form));
      alert('Unable to save the query, please reach out to us via mail or phone number')
    },
  }
};
</script>

<style scoped>
.heading {
  font-size: calc(22px + (26 -22) * ((100vw - 300px) / (1600 - 300)));
  font-weight: bold;
}
a {
  color: inherit;
}
.wrapper {
  background-color: rgb(255, 255, 255, 0.7);
}
#contact {
  background-repeat: no-repeat;
  display: table;
  width: 100%;
  height: 100vh;
  background: url("./../assets/network.jpg") top center;
  background-size: cover;
}
</style>