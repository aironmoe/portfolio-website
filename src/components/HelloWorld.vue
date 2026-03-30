<script setup>
import { ref } from "vue";
import imgprofile from "../assets/portfolio.jpg";
const count = ref(0);
const isZoomed = ref(false);
</script>

<template>
  <div>
    <section id="center">
      <div class="card">
        <div class="fb-card-header">
          <img
            :src="imgprofile"
            class="fb-avatar"
            :class="{ zoomed: isZoomed }"
            @click="isZoomed = !isZoomed"
          />

          <div>
            <h3 class="fb-name">Airon Moe T. Oquindo</h3>
            <p class="fb-date">The Full Stack Dev You need</p>
            <br />
          </div>
        </div>

        <div class="fb-card-content">
          <p>
            A motivated individual with 2 years experience in building and maintaining
            system solutions, focused on continuous improvement and delivering value to
            the organization.
          </p>
        </div>
        <div class="fb-actions">
          <button @click="count++">👍 Like {{ count }}</button>
        </div>
      </div>

      <div class="card">
        <h2>Work Experience</h2>
        <h4 class="fb-name">
          Junior RPA Developer at Wilcon Depot Inc. from (August 29, 2024 to Present)
        </h4>
        <p>
          Junior RPA Developer I am currently working at Wilcon Depot Inc. as a Robotic
          Process Automation (RPA)Developer, where I am responsible for developing,
          maintaining, and improving their automation processes using RAX and N8N. My role
          involves streamliningrepetitive asks of other business aaunits, managing
          automation-related data, and supporting business efficiency through intelligent
          automation solutions
        </p>
        <h4 class="fb-name">
          Fatima University Medical Center(February 5 2024 - April 5 2024 )
        </h4>
        <p>
          System Developer Carried on developing a web-based inventory management system
          using PHP and MySQL, which involved designing and implementing database
          structures,creating dynamic user interfaces,optimizing application performance
          and ensuring system reliability and data accuracy throughout development process
        </p>
      </div>
      
      <div class="card">
        <div class="fb-name">Education</div>
        <h4 class="fb-name">Our Lady of Fatima University</h4>
        <p class="fb-date">College</p>
        <p>
          Our lady of Fatima University 2020 - 2024 Bachelor of Science Information
          Technology
        </p>
      </div>
    </section>
  </div>
</template>
