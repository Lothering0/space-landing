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

    <div class="curve mercury"></div>
    <div class="planet mercury"></div>

    <InfoBlock marginTop="166">
      <template v-slot:h1>
        <h1>Mercury</h1>
      </template>

      <template v-slot:p>
        <p><i>Mercury</i> — the smallest planet in our solar system and closest to the <i>Sun</i> — is only slightly larger than <i>Earth's Moon</i>. <i>Mercury</i> is the fastest planet, zipping around the <i>Sun</i> every 88 <i>Earth</i> days.</p>
      </template>
    </InfoBlock>

    <div class="curve venus"></div>
    <div class="planet venus"></div>

    <InfoBlock marginTop="438">
      <template v-slot:h1>
        <h1>Venus</h1>
      </template>

      <template v-slot:p>
        <p><i>Venus</i> spins slowly in the opposite direction from most planets. A thick atmosphere traps heat in a runaway greenhouse effect, making it the hottest planet in our solar system.</p>
      </template>
    </InfoBlock>

    <div class="curve earth"></div>
    <Moon
      name="Moon"
      top="3479px"
      left="131px"
      backgroundColor="#1d1f2f"
    />
    <div class="planet earth"></div>

    <InfoBlock marginTop="229">
      <template v-slot:h1>
        <h1>Earth</h1>
      </template>

      <template v-slot:p>
        <p><i>Earth</i> — our home planet — is the only place we know of so far that’s inhabited by living things. It's also the only planet in our solar system with liquid water on the surface.</p>
      </template>
    </InfoBlock>

    <div class="curve mars"></div>
    <Moon
      name="Phobos"
      top="4446px"
      left="990px"
    />
    <Moon
      name="Deimos"
      top="4505px"
      left="1258px"
    />
    <div class="planet mars"></div>

    <InfoBlock marginTop="424">
      <template v-slot:h1>
        <h1>Mars</h1>
      </template>

      <template v-slot:p>
        <p><i>Mars</i> is a dusty, cold, desert world with a very thin atmosphere. There is strong evidence <i>Mars</i> was — billions of years ago — wetter and warmer, with a thicker atmosphere.</p>
      </template>
    </InfoBlock>

    <div class="curve jupiter"></div>
    <Moon
      name="Europa"
      top="4752px"
      left="1357px"
      backgroundColor="#121222"
    />
    <Moon
      name="Ganymede"
      top="4995px"
      left="1259px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Io"
      top="5591px"
      left="1226px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Callisto"
      top="5869px"
      left="1258px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Valetudo"
      top="6153px"
      left="1307px"
      backgroundColor="#11101f"
    />
    <div class="planet jupiter"></div>

    <InfoBlock marginTop="396">
      <template v-slot:h1>
        <h1>Jupiter</h1>
      </template>

      <template v-slot:p>
        <p><i>Jupiter</i> is more than twice as massive than the other planets of our solar system combined. The giant planet's Great Red spot is a centuries-old storm bigger than <i>Earth</i>.</p>
      </template>
    </InfoBlock>

    <div class="curve saturn"></div>
    <Moon
      name="Dione"
      top="6043px"
      left="123px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Mimas"
      top="6084px"
      left="293px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Titan"
      top="6102px"
      left="1063px"
      backgroundColor="#11101f"
    />
    <div class="planet saturn"></div>

    <InfoBlock marginTop="463">
      <template v-slot:h1>
        <h1>Saturn</h1>
      </template>

      <template v-slot:p>
        <p>Adorned with a dazzling, complex system of icy rings, <i>Saturn</i> is unique in our solar system. The other giant planets have rings, but none are as spectacular as <i>Saturn's</i>.</p>
      </template>
    </InfoBlock>

    <div class="curve uranus"></div>
    <Moon
      name="Umbriel"
      top="6385px"
      left="155px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Titania"
      top="6646px"
      left="219px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Oberon"
      top="7255px"
      left="229px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Miranda"
      top="7502px"
      left="166px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Puck"
      top="7744px"
      left="106px"
      backgroundColor="#11101f"
    />
    <div class="planet uranus"></div>

    <InfoBlock marginTop="427">
      <template v-slot:h1>
        <h1>Uranus</h1>
      </template>

      <template v-slot:p>
        <p><i>Uranus</i> — seventh planet from the <i>Sun</i> — rotates at a nearly 90-degree angle from the plane of its orbit. This unique tilt makes <i>Uranus</i> appear to spin on its side.</p>
      </template>
    </InfoBlock>

    <div class="curve neptune"></div>
    <Moon
      name="Proteus"
      top="7911px"
      left="243px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Triton"
      top="7863px"
      left="1103px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Hippocamp"
      top="7897px"
      left="1241px"
      backgroundColor="#11101f"
    />
    <Moon
      name="Nereid"
      top="7952px"
      left="1457px"
      backgroundColor="#11101f"
    />
    <div class="planet neptune"></div>

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
  position: absolute !important;
  top: 52px;
  right: 91px;
  background-color: #13111c;
  border-radius: 5px;
}

.white-space {
  height: 404px;
}

.curve {
  position: absolute;

  width: 100%;
  height: 200px;

  background-image: url('@/static/curve-horizontal.svg');
  background-repeat: no-repeat;
  background-size: 100%;
}

.curve.mercury {
  margin-top: 41px;
}

.curve.venus {
  margin-top: 221px;
  transform: rotate(180deg);
}

.curve.earth, .curve.jupiter, .curve.uranus {
  height: 2093px;
  width: 281px;

  background-image: url('@/static/curve-vertical.svg');
  background-position: center;
}

.curve.earth {
  top: 3062px;
}

.curve.mars {
  margin-top: 333px;
}

.curve.jupiter {
  top: 4489px;
  right: 0;

  transform: rotate(180deg);
}

.curve.saturn {
  top: 6002px;

  transform: rotate(180deg);
}

.curve.uranus {
  top: 5958px;
}

.curve.neptune {
  margin-top: 375px;
}

.planet {
  position: absolute;

  width: 336px;
  height: 336px;
}

.planet.mercury {
  margin-top: -25px;
  left: 132px;
}

.planet.venus {
  margin-top: 229px;
  left: 856px;
}

.planet.earth {
  margin-top: 259px;
  left: 113px;
}

.planet.mars {
  margin-top: 229px;
  left: 585px;
}

.planet.jupiter {
  margin-top: 229px;
  right: 149px;
}

.planet.saturn {
  margin-top: 229px;
  right: 581px;
}

.planet.uranus {
  margin-top: 229px;
  left: 153px;
}

.planet.neptune {
  margin-top: 229px;
  right: 570px;
}
</style>
