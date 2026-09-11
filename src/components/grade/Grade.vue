<template>
  <div class="grade-page">
    <v-container>
      <v-card
        class="grade-card"
        flat
      >
        <v-card-text class="grade-content">

          <div class="grade-title">
            Grade Evaluation
          </div>

          <div class="grade-description">
            Enter your score to evaluate your grade.
          </div>

          <v-text-field
            v-model="score"
            label="Enter your score"
            type="number"
            min="0"
            max="100"
            outlined
            dense
            class="score-input"
          />

          <v-btn
            block
            class="evaluate-btn"
            @click="evaluateGrade"
          >
            Evaluate
          </v-btn>

          <div
            v-if="grade"
            class="result"
          >
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

      if (score < 0 || score > 100 || this.score === '') {
        this.grade = 'Invalid score'
        return
      }

      if (score >= 80) {
        this.grade = 'A'
      } else if (score >= 70) {
        this.grade = 'B'
      } else if (score >= 60) {
        this.grade = 'C'
      } else if (score >= 50) {
        this.grade = 'D'
      } else {
        this.grade = 'F'
      }
    }
  }
}
</script>

<style scoped>
.grade-page {
  width: 100%;
}

.grade-card {
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  border-radius: 18px;
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12) !important;
}

.grade-content {
  padding: 20px;
}

.grade-title {
  margin-bottom: 6px;
  font-size: 13px;
  font-weight: 700;
  color: #333333;
}

.grade-description {
  margin-bottom: 16px;
  font-size: 12px;
  line-height: 1.7;
  color: #777777;
}

.score-input {
  margin-bottom: 8px;
}

.evaluate-btn {
  height: 42px !important;
  border-radius: 10px;
  font-size: 12px;
  font-weight: 600;
  text-transform: none;
}

.result {
  margin-top: 18px;
  padding: 12px 16px;
  border-radius: 10px;
  background: #f5f5f5;
  text-align: center;
  font-size: 14px;
  font-weight: 700;
  color: #333333;
}
</style>
