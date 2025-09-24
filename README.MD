# 📊 Grade Calculator Package (esepunittests)

This package provides a simple `GradeCalculator` utility written in Go for calculating a weighted final course grade based on **assignments**, **exams**, and **essays**, and converting that numerical score into a letter grade.

---

## 🚀 Getting Started

### 📦 Installation

Since this is a single package, you can typically place the Go files within a directory named `esepunittests` in your Go workspace. Runtime requirements: Golang 1.24+

### 📝 Usage

The primary entry point is the `NewGradeCalculator` function.  

You then use the `AddGrade` method to input student scores. The `calculateNumericalGrade` weighs the essay, exam, and assignment categories in order to assign an overall numeric value. Lastly. the `GetFinalGrade` function calculates the result as a letter grade.

### 📝 Testing
Run unit tests:
```
cd grade_calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade_calculator/
go test -coverprofile=coverage.txt ./...
```