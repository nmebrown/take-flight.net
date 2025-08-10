<template>
  <section class="work">
    <h1>Past Projects</h1>

    <div class="showcase">
      <div class="card featured howesound">
        <a href="http://www.sustainablehowesound.ca" target="_blank">
          <h4>Save the Howe Sound</h4>
        </a>
      </div>
      <div class="card htc">
        <a href="http://www.houstontrust.com" target="_blank">
          <h4>Houston Trust Company</h4>
        </a>
      </div>
      <div class="card salishsea">
        <a href="http://www.salishseaaction.org" target="_blank">
          <h4>Save the Salish Sea</h4>
        </a>
      </div>
      <div class="card tal">
        <a href="http://www.thealbertalibrary.ab.ca" target="_blank">
          <h4>The Alberta Library</h4>
        </a>
      </div>
      <div class="card bctransplant">
        <a href="http://www.transplant.bc.ca" target="_blank">
          <h4>BC Transplant</h4>
        </a>
      </div>
      <div class="card tf">
        <a href="http://www.take-flight.net" target="_blank">
          <h4>Take Flight</h4>
        </a>
      </div>
      <div class="card featured noomii">
        <a href="http://www.noomii.com" target="_blank"><h4>Noomii.com</h4></a>
      </div>
      <div class="card aven">
        <a href="http://www.asexuality.org" target="_blank">
          <h4>Asexual Visibility & Education Network</h4>
        </a>
      </div>
    </div>
  </section>
</template>

<style>
.showcase {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 20px;
  margin: 0;
}

.card {
  background: #ddd;
  border: 2px solid #eee;
  border-radius: 1px;
  height: 8em;
  margin: 0;
  position: relative;
  width: 100%;

  h4 {
    background: rgba(238, 238, 238, 0.95);
    margin: 0;
    padding: 1em 1em;
    position: absolute;
    bottom: 0;
    width: 100%;
    transition: background 0.5s;

    &:hover {
      background: #fff;
    }
  }

  &.aven {
    background: url('@/assets/images/sites/aven.png') no-repeat;
    background-size: cover;
  }
  &.bctransplant {
    background: url('@/assets/images/sites/bctransplant.png') no-repeat;
    background-size: cover;
  }
  &.howesound {
    background: url('@/assets/images/sites/howesound.png') no-repeat;
    background-size: cover;
  }
  &.htc {
    background: url('@/assets/images/sites/htc.png') no-repeat;
    background-size: cover;
  }
  &.noomii {
    background: url('@/assets/images/sites/noomii.png') no-repeat;
    background-size: cover;
  }
  &.salishsea {
    background: url('@/assets/images/sites/salishsea.png') no-repeat;
    background-size: cover;
  }
  &.tal {
    background: url('@/assets/images/sites/tal.png') no-repeat;
    background-size: cover;
  }
  &.tf {
    background: url('@/assets/images/sites/tf.png') no-repeat;
    background-size: cover;
  }
}
</style>
