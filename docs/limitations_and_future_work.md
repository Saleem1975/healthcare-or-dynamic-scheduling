# Limitations and Future Work

## Limitations

### 1. Limited test schedule size

The paper compared traditional static scheduling and CNN-based dynamic scheduling using ten test videos. This provided a useful demonstration, but a larger dataset would be needed to establish stronger statistical evidence.

### 2. No confidence intervals or hypothesis tests

Because of the limited number of test surgeries, the authors did not construct confidence intervals or conduct hypothesis tests for the reduction in idle time and waiting time.

### 3. Misclassification risk

The CNN sometimes misclassified images with rolled white retrieval bags as the end of Phase 4. This could delay the schedule update and increase phase-detection error.

### 4. Procedure-specific validation

The study focused on laparoscopic cholecystectomy. Although the method can be adapted to other laparoscopic procedures, additional validation would be required before broader deployment.

### 5. Clinical deployment requirements

The model should not be treated as a ready-to-deploy clinical system. Real-world use would require hospital validation, clinical review, system integration, privacy safeguards, and appropriate approval processes.

## Future work

Future research and implementation work may include:

- Expanding the dataset with more surgical videos
- Improving the CNN architecture
- Testing other deep learning architectures
- Adding more contextual operational variables
- Validating the model across different hospitals
- Applying the method to other laparoscopic surgeries, such as appendectomy and hernia repair
- Integrating the prediction model with hospital scheduling systems
- Developing dashboards for real-time OR monitoring
