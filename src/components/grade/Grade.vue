<template>
  <div class="grade-page">
    <v-container>
      <v-card class="grade-card" flat>
        <v-card-title>
          Grade Evaluation
        </v-card-title>

        <v-card-text>
          <v-text-field
            v-model="score"
            label="Enter your score"
            type="number"
            outlined
          />

          <v-btn
            block
            @click="evaluateGrade"
          >
            Evaluate
          </v-btn>

          <div v-if="grade" class="result">
            Grade: {{ grade }}
          </div>
        </v-card-text>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'Grade_Eva',

  data() {
    return {
      score: '',
      grade: ''
    }
  },

  methods: {
    evaluateGrade() {
      const score = Number(this.score)
      if (score >= 80) {
        this.grade = 'A'
      } else if (score >= 70) {
        this.grade = 'B'
      } else if (score >= 60) {
        this.grade = 'C'
      } else {
        this.grade = 'D'
      }
    }
  }
}
</script>