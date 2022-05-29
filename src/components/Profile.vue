<template>
  <div>
    <div class="d-flex justify-content-center align-center">
      <img src="../assets/profilepic.png" class="profile-pic" />
    </div>
    <div class="mt-3 text-center font-weight-bold">
      <h2 class="font-weight-bold">Profissional de Educação Física</h2>
      <h3 class="font-weight-bold">Personal Trainer</h3>
      <h4 class="font-weight-bold">
        Coach <span>@crossbox300</span> & <span>@blackfitacademia</span>
      </h4>
      <p class="border-bottom">CREF: 9445-G/PA</p>
    </div>
    <div class="d-flex justify-center align-center pt-6">
      <a href="#about">
        <img
          class="zoom-in-out-box"
          src="../assets/arrow-down.png"
          width="50"
        />
      </a>
    </div>
  </div>
</template>

<style scoped>
.border-bottom {
  border-bottom: 1px solid #313552;
}

span {
  /* link blue */
  color: #00a0d2;
}

p {
  font-weight: 600;
}

.profile-pic {
  width: 70%;
  border-radius: 50%;
  border: 3px solid #313552;
}

/* .zoom-in-out-box {
  animation: zoom-in-zoom-out 1s ease infinite;
}

@keyframes zoom-in-zoom-out {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(1.1, 1.1);
  }
  100% {
    transform: scale(1, 1);
  }
} */
</style>
