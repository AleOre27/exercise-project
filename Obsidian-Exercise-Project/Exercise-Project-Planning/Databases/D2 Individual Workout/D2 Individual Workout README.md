![[D2 Columns]]![[D2 template|1000]]

Column Specification
---

| **Column**  | Properties                        | Purpose                                                               | DataType | Input     | Possible Input                 |
| ----------- | --------------------------------- | --------------------------------------------------------------------- | -------- | --------- | ------------------------------ |
| ID          | primary key                       | Identification                                                        | Integer  | Auto      | Auto                           |
| Focus       | D1.2 Focus: Dependent on D2 Focus | Identify main goal (ie: legs and back)                                | Text     | Fill      | Fill                           |
| Group       |                                   | General subset within focus (ie: upper leg)                           | Text     | Fill      | Fill                           |
| Muscle      |                                   | Identify what muscle is being used                                    | Text     | Fill      | Fill                           |
| Exercise    |                                   | Specified exercise (ie: Dumbbell curl)                                | Text     | Fill      | Fill                           |
| Sets        |                                   | Set for exercise                                                      | Integer  | Fill      | Fill                           |
| Reps        |                                   | Repetitions of exercise                                               | Integer  | Fill      | Fill                           |
| Measurments |                                   | How the exercise is accounted for                                     | Text     | Drop-down | Count, Time                    |
| Weight      |                                   | Weight of used. When body weight is not chosen then allows an integer | Text     | Drop-down | Body weight, otherwise integer |
| Structure   |                                   | Whether you do one side or both at the same time                      | Text     | Drop-down | Symmetric, Asymmetric          |

![[D2 Dependency]]
Once a Focus is chosen
- Then Group is chosen
- Finally allows to choose muscle

Measurement:
- Time
- Count
- Till Failure

Equipment:
- Enter New Equipment
- Body Weight
- Dumbbell
- etc.
	- Dependent on D1 Equipment column

Weight:
- **When Equipment is body weight**
- Enter number in pounds

Structure:
- Symmetrical
- Asymmetrical 

When exercise is chosen:
What should autofill but can be changed
- Measurement
- Equipment
- Structure 