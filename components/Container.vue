<template>
  <div class="container">
    <SolarSystem />

    <InfoBlock class="solar-system-info">
      <template v-slot:h1>
        <h1>Sun</h1>
      </template>

      <template v-slot:p>
        <p>The <i>Sun</i> is a yellow dwarf star, a hot ball of glowing gases at the heart of our solar system. Its gravity holds everything from the biggest planets to tiny debris in its orbit.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="200">
      <template v-slot:h1>
        <h1>Mercury</h1>
      </template>

      <template v-slot:p>
        <p><i>Mercury</i> — the smallest planet in our solar system and closest to the <i>Sun</i> — is only slightly larger than <i>Earth's Moon</i>. <i>Mercury</i> is the fastest planet, zipping around the <i>Sun</i> every 88 <i>Earth</i> days.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="438">
      <template v-slot:h1>
        <h1>Venus</h1>
      </template>

      <template v-slot:p>
        <p><i>Venus</i> spins slowly in the opposite direction from most planets. A thick atmosphere traps heat in a runaway greenhouse effect, making it the hottest planet in our solar system.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="229">
      <template v-slot:h1>
        <h1>Earth</h1>
      </template>

      <template v-slot:p>
        <p><i>Earth</i> — our home planet — is the only place we know of so far that’s inhabited by living things. It's also the only planet in our solar system with liquid water on the surface.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="424">
      <template v-slot:h1>
        <h1>Mars</h1>
      </template>

      <template v-slot:p>
        <p><i>Mars</i> is a dusty, cold, desert world with a very thin atmosphere. There is strong evidence <i>Mars</i> was — billions of years ago — wetter and warmer, with a thicker atmosphere.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="396">
      <template v-slot:h1>
        <h1>Jupiter</h1>
      </template>

      <template v-slot:p>
        <p><i>Jupiter</i> is more than twice as massive than the other planets of our solar system combined. The giant planet's Great Red spot is a centuries-old storm bigger than <i>Earth</i>.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="463">
      <template v-slot:h1>
        <h1>Saturn</h1>
      </template>

      <template v-slot:p>
        <p>Adorned with a dazzling, complex system of icy rings, <i>Saturn</i> is unique in our solar system. The other giant planets have rings, but none are as spectacular as <i>Saturn's</i>.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="427">
      <template v-slot:h1>
        <h1>Uranus</h1>
      </template>

      <template v-slot:p>
        <p><i>Uranus</i> — seventh planet from the <i>Sun</i> — rotates at a nearly 90-degree angle from the plane of its orbit. This unique tilt makes <i>Uranus</i> appear to spin on its side.</p>
      </template>
    </InfoBlock>

    <InfoBlock marginTop="438">
      <template v-slot:h1>
        <h1>Neptune</h1>
      </template>

      <template v-slot:p>
        <p><i>Neptune</i> — the eighth and most distant major planet orbiting our <i>Sun</i> — is dark, cold and whipped by supersonic winds. It was the first planet located through mathematical calculations, rather than by telescope.</p>
      </template>
    </InfoBlock>

    <div class="white-space"></div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  position: relative;
  background-image: linear-gradient(180deg, #13111C 10.94%, #202334 35.68%, #0F0E1D 61.71%);
}

.solar-system-info {
  position: absolute;
  top: 52px;
  right: 91px;
  background-color: #13111c;
  border-radius: 5px;
}

.white-space {
  height: 404px;
}
</style>
