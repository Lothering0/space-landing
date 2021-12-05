<template>
  <div class="container">
    <SolarSystem />

    <div class="stars" id="stars-1">
      <div class="stars-image"></div>
    </div>

    <InfoBlock class="solar-system-info" id="start">
      <template v-slot:h1>
        <h1>Sun</h1>
      </template>

      <template v-slot:p>
        <p>The <i>Sun</i> is a yellow dwarf star, a hot ball of glowing gases at the heart of our solar system. Its gravity holds everything from the biggest planets to tiny debris in its orbit.</p>
      </template>
    </InfoBlock>

    <div class="curve mercury"></div>
    <div class="planet mercury"></div>

    <div class="stars" id="stars-2">
      <div class="stars-image"></div>
    </div>

    <InfoBlock marginTop="166" id="mercury">
      <template v-slot:h1>
        <h1>Mercury</h1>
      </template>

      <template v-slot:p>
        <p><i>Mercury</i> — the smallest planet in our solar system and closest to the <i>Sun</i> — is only slightly larger than <i>Earth's Moon</i>. <i>Mercury</i> is the fastest planet, zipping around the <i>Sun</i> every 88 <i>Earth</i> days.</p>
      </template>
    </InfoBlock>

    <div class="curve venus"></div>
    <div class="planet venus"></div>

    <InfoBlock marginTop="438" id="venus">
      <template v-slot:h1>
        <h1>Venus</h1>
      </template>

      <template v-slot:p>
        <p><i>Venus</i> spins slowly in the opposite direction from most planets. A thick atmosphere traps heat in a runaway greenhouse effect, making it the hottest planet in our solar system.</p>
      </template>
    </InfoBlock>

    <div class="stars" id="stars-3">
      <div class="stars-image"></div>
    </div>

    <div class="curve earth"></div>
    <Moon
      name="Moon"
      top="3479px"
      left="131px"
      backgroundColor="#1d1f2f"
    />
    <div class="planet earth"></div>

    <InfoBlock marginTop="229" id="earth">
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

    <InfoBlock marginTop="424" id="mars">
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
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Callisto"
      top="5869px"
      left="1258px"
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Valetudo"
      top="6153px"
      left="1307px"
      backgroundColor="#0f0e1d"
    />
    <div class="planet jupiter"></div>

    <InfoBlock marginTop="396" id="jupiter">
      <template v-slot:h1>
        <h1>Jupiter</h1>
      </template>

      <template v-slot:p>
        <p><i>Jupiter</i> is more than twice as massive than the other planets of our solar system combined. The giant planet's Great Red spot is a centuries-old storm bigger than <i>Earth</i>.</p>
      </template>
    </InfoBlock>

    <div class="stars" id="stars-4">
      <div class="stars-image"></div>
    </div>

    <div class="curve saturn"></div>
    <Moon
      name="Dione"
      top="6043px"
      left="123px"
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Mimas"
      top="6084px"
      left="293px"
    />
    <Moon
      name="Titan"
      top="6102px"
      left="1063px"
    />
    <div class="planet saturn"></div>

    <InfoBlock marginTop="463" id="saturn">
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
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Titania"
      top="6646px"
      left="219px"
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Oberon"
      top="7255px"
      left="229px"
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Miranda"
      top="7502px"
      left="166px"
      backgroundColor="#0f0e1d"
    />
    <Moon
      name="Puck"
      top="7744px"
      left="106px"
      backgroundColor="#0f0e1d"
    />
    <div class="planet uranus"></div>

    <div class="stars" id="stars-5">
      <div class="stars-image"></div>
    </div>

    <InfoBlock marginTop="427" id="uranus">
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
    />
    <Moon
      name="Triton"
      top="7863px"
      left="1103px"
    />
    <Moon
      name="Hippocamp"
      top="7897px"
      left="1241px"
    />
    <Moon
      name="Nereid"
      top="7952px"
      left="1457px"
    />
    <div class="planet neptune"></div>

    <InfoBlock marginTop="438" id="neptune">
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

  background-image: url('@/static/curves/curve-horizontal.svg');
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

  background-image: url('@/static/curves/curve-vertical-1.svg');
  background-position: center;
}

.curve.earth {
  top: 3062px;
}

.curve.mars {
  margin-top: 333px;
}

.curve.jupiter {
  width: 317px;
  height: 2199px;

  top: 4467px;
  right: 0;

  background-image: url('@/static/curves/curve-vertical-2.svg');
}

.curve.saturn {
  top: 6002px;

  transform: rotate(180deg);
}

.curve.uranus {
  top: 5958px;
  width: 321px;
  height: 2209px;

  background-image: url('@/static/curves/curve-vertical-3.svg');
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

.stars {
  position: absolute;

  width: 389px;
  height: 389px;

  display: flex;

  background-image: radial-gradient(50% 50% at 50% 50%, rgba(255, 217, 96, 0.1) 0%, rgba(255, 217, 96, 0) 100%);
  background-repeat: no-repeat;
  background-position: 50% 50%;

  animation: 2s linear 0s infinite alternate shining;

  .stars-image {
    width: 142px;
    height: 142px;

    background-size: cover;

    margin: auto;
  }
}

@keyframes shining {
  from {
    background-size: 75% 75%;
  }
  to {
    background-size: 100% 100%;
  }
}

#stars-1 {
  top: 1693px;
  right: 81px;

  .stars-image {
    background-image: url('@/static/stars/stars-1.png');
  }
}

#stars-2 {
  top: 2508px;

  .stars-image {
    background-image: url('@/static/stars/stars-2.png');
  }
}

#stars-3 {
  top: 3518px;
  right: 10px;

  .stars-image {
    background-image: url('@/static/stars/shining.png');
  }
}

#stars-4 {
  top: 5568px;
  left: -19px;

  .stars-image {
    background-image: url('@/static/stars/shooting-star.png');
  }
}

#stars-5 {
  top: 6747px;
  right: 92px;

  .stars-image {
    background-image: url('@/static/stars/glare.png');
  }
}
</style>
