<template>
  <div class="solutions">
    <div class="solutions_header">
      <h2>Solutions and Services</h2>
      <p>
        Forgery and tamperying cost people and organisations billions of dollars
        around the world. Protect your personal signature and your
        organisation's official seal from being faked, forged or mimicked by
        fraudsters by using the Veryfy Seal.
      </p>
    </div>
    <div class="service_container">
      <div>
        <Service
          title="Secure Cert"
          cl="service"
          text="Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal."
        >
          <template v-slot:header>
            <MarkerCheck class="icon"></MarkerCheck>
          </template>
        </Service>
      </div>
      <div class="service">
        <Service
          title="Process Control"
          cl="service"
          text="Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal."
        >
          <template v-slot:header>
            <ControllerClassic class="icon"></ControllerClassic>
          </template>
        </Service>
      </div>
      <div class="service">
        <Service
          title="Automated Forms Processing"
          cl="service"
          text="Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal."
        >
          <template v-slot:header>
            <HomeAutomation class="icon"></HomeAutomation>
          </template>
        </Service>
      </div>
      <div>
        <Service
          title="Smart Invoice"
          cl="service"
          text="Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal."
        >
          <template v-slot:header>
            <SmartCard class="icon"></SmartCard>
          </template>
        </Service>
      </div>
    </div>
  </div>
</template>

<script>
import {
  MarkerCheck,
  HomeAutomation,
  ControllerClassic,
  SmartCard,
} from "mdue";
import Service from "./Service.vue";

export default {
  components: {
    MarkerCheck,
    HomeAutomation,
    ControllerClassic,
    SmartCard,
    Service,
  },
  data() {
    return {
      services: [
        {
          icon: "",
          title: "Secure Cert",
          text: `Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal`,
        },
        {
          icon: "",
          title: "Process Control",
          text: `Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal`,
        },
        {
          icon: "",
          title: "Automated Forms Processing",
          text: `Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal`,
        },
        {
          icon: "",
          title: "Smart Invoice",
          text: `Protect your valuable documents like certificates, diplomats
            transcripts and show tickets from tampering by adding a unique
            Veryfy Seal`,
        },
      ],
    };
  },
};
</script>

<style>
.solutions {
  width: 90%;
  margin: 80px auto;
}
.icon {
  width: 200px;
  color: var(--btn_color--);
  height: 80px;
  margin: 10px 0;
}

.service {
  margin-bottom: 20px;
}

@media (min-width: 990px) {
  .solutions {
    padding-top: 50px;
    text-align: left;
    width: 80%;
  }

  .solutions_header > h2 {
    font-weight: 800;
  }

  .service_container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
    margin-top: 50px;
  }

  .service_icon {
    width: 150px;
  }
  .service_content {
    width: 80%;
  }

  .service_content > h4 {
    font-weight: 700;
  }

  .service {
    display: flex;
    width: 100%;
  }
}
</style>
