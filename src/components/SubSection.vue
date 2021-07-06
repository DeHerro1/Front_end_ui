<template>
  <div class="sub_section">
    <div class="design_right"></div>
    <div class="design_left"></div>
    <div class="sub_section_content">
      <h2>Document Verification Made Easy</h2>
      <p>
        The greatest platform for securing documents.
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.sub_section {
  background: var(--default_color--);
  color: white;
  padding: 50px 0;
  width: 100%;
  position: relative;
  z-index: -1;
}
.sub_section_content {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.sub_section_content > p {
  margin: 0;
}

.design_right,
.design_left {
  display: none;
}

.sub_section_content > h2 {
  font-weight: 700;
}

@media (min-width: 990px) {
  .sub_section {
    overflow: hidden;
  }
  .design_right {
    display: block;
    position: absolute;
    right: -140px;
    width: 200px;
    height: 200px;
    background: #38326c;
    border-radius: 20px;
    transform: rotate(60deg);
  }

  .sub_section_content > h2 {
    font-weight: 800;
    font-size: 2rem;
  }

  .design_left {
    display: block;
    position: absolute;
    top: 20px;
    left: -150px;
    width: 250px;
    height: 250px;
    background: #38326c;
    border-radius: 20px;
    transform: rotate(60deg);
  }
}
</style>
