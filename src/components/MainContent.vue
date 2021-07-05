<template>
  <div class="main_content">
    <div class="img_container">
      <img src="../assets/staff.jpg" alt="staff" class="content_img" />
    </div>
    <div class="main_text">
      <h2>How it Works</h2>
      <p>
        Veryfy provides you with a single platform to control every process in
        your organisation through a clever document-centric workflow oversight
        system that also denfends your external image by extending beyond your
        four walls,
      </p>
      <div class="main_control">
        <h3>Control Every Process</h3>
        <p>
          Veryfy is indispensable in the modern organisation because every
          organisation is under constant threat of subversion from within and
          without. Even organisations that pride themselves on their culture of
          high trust and internal solidarity understand that it only takes one
          bad nut to ruin it for everyone. In fact, the higher the level of
          internal trust, the more vulnerable the organisation is to deliberate
          sabotage, corruption and subterfuge. For such organisations to
          maintain the high degree of internal trust and cohesion they thrive
          on, the right kind of tool that does not disrupt the culture is
          required. Veryfy is that subtle but immensely powerful swiss army
          knife cutting through bureaucracy to protect the essential
          reputational assets of the organisation.
        </p>
      </div>
      <div class="main_control">
        <h3>Audit Trail</h3>
        <p>
          Automatically create a complete audit trail of all activities, The
          Veryfy system is setup to automatically monitor all activities
          including user identities of who created transaction, and any user who
          modified the record.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.main_content {
  width: 100%;
  padding: 50px 0;
  display: flex;
  flex-direction: column;
}

.main_text > h2 {
  font-weight: 700;
  text-align: center;
}

.main_control > h3 {
  text-align: center;
}

.main_text {
  text-align: left;
}

.content_img {
  width: 100%;
}

@media (min-width: 768px) {
  .main_content {
    display: flex;
    text-align: left;
  }

  .main_control > p {
    padding-left: 20px;
  }
}

@media (min-width: 990px) {
  .main_content {
    display: flex;
    text-align: left;
    flex-direction: row;
  }

  .img_container {
    width: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .main_text > h2 {
    font-weight: 700;
  }

  .main_control > h3,
  .main_text > h2 {
    text-align: left;
  }

  .main_control > h3 {
    text-align: left;
  }

  .main_text {
    width: 100%;
  }

  .main_control > p {
    padding-left: 20px;
  }
}
</style>
