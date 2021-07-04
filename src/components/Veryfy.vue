<template>
  <div class="veryfy">
    <div class="veryfy_head">
      <h2>Why Use Veryfy</h2>
      <p>
        Get your entire organisation and business process IN & UNDER CONTROL
        using the one-stop solution that prevents evasion of critical processes
        through fraud, forgery, misrepresentation, pure deception and evidence
        fabrication. What is more, Veryfy extends beyond your four walls by
        providing public portals through which partners, suppliers, agents, and
        even the general public can obtain instant assurance that specific
        actions, representations, warranties, claims, statements,
        correspondence, processes and operations have been properly and duly
        authorised by the relevant Directors and Managers within your
        organisation.
      </p>
    </div>
    <div class="veryfy_main_content">
      <div>
        <Service
          title="Sign Up is Free"
          cl="veryfy_content"
          text="You don’t pay a dime. Once you have fully configured the platform to
            suit your need, you only pay per use for value-added transactions
            with direct, measurable, benefits. If we are not adding to the
            bottomline, you don’t fork out a penny."
        >
          <template v-slot:header>
            <div>
              <img src="../assets/lap1.jpg" alt="laptop1" class="laptops" />
            </div>
          </template>
        </Service>
      </div>
      <div>
        <Service
          title="Fully Cloud-Hosted"
          cl="veryfy_content"
          text="You don’t have to worry about the cost of infrastructure,
            cybersecurity for transactional servers, uptime management, or
            system administrators. We take care of all of that for you. It is
            our specialty; feel free to leave it in our hands."
        >
          <template v-slot:header>
            <div>
              <img src="../assets/lap2.jpg" alt="laptop2" class="laptops" />
            </div>
          </template>
        </Service>
      </div>
      <div>
        <Service
          title="Fully-Featured Web-Based ERP"
          cl="veryfy_content"
          text="Ever evolving role dynamics, multi-level permissions, interwoven
            reporting lines, etc. Set up departments, sub-admins, oversight
            layers and all the key managerial mechanics using the powerful but
            highly intuitive interfaces."
        >
          <template v-slot:header>
            <div>
              <img src="../assets/lap3.jpg" alt="laptop2" class="laptops" />
            </div>
          </template>
        </Service>
      </div>
      -->
    </div>
  </div>
</template>

<script>
import Service from "./Service.vue";

export default {
  components: { Service },
};
</script>

<style scoped>
.veryfy {
  padding: 50px 20px;
}
.veryfy_head > h2 {
  text-align: left;
  font-weight: 800;
}

.laptops {
  width: 200px;
  height: 200px;
  margin: 0 0 40px 0;
}

.veryfy_head {
  margin-bottom: 100px;
  text-align: left;
}

h3 {
  font-weight: 600;
}

@media (min-width: 768px) {
  .veryfy_main_content {
    display: flex;
    padding: 0 20px;
  }

  .veryfy_content {
    margin-right: 10px;
  }
}
</style>
