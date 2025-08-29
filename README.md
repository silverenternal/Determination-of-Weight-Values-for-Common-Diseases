Determination of Weight Values for Common Diseases
This project contains a Python dictionary that maps common disease names and medical histories to weight values (ranging from 1 to 10). These weights are intended to quantify the potential impact of specific medical conditions on a patient's stability during medical transport (e.g., ambulance transfer, inter-hospital transfer).

Project Origin
This weight assignment system was developed as part of a research initiative to assess and quantify risks associated with patient transport. The theoretical basis and justification for these weights are detailed in the accompanying theoretical_basis.txt document.

Contents
disease_weights.py: A Python file containing the disease_weights dictionary.
theoretical_basis.txt: A comprehensive report (in Chinese) explaining the rationale behind the assigned weight values, based on clinical knowledge and available medical literature.
Usage
The primary purpose of this dictionary is to serve as a reference for medical professionals or researchers evaluating patient risk during transport. It can be integrated into larger systems for patient assessment and triage.

Example (Python)
# Import the dictionary
from disease_weights import disease_weights

# Get the weight for a specific condition
condition = "心梗" # Myocardial Infarction
weight = disease_weights.get(condition, 1) # Default weight is 1 if not found

print(f"The weight for '{condition}' is {weight}.")
Note on Accuracy and Validation
While the weights have been assigned based on clinical reasoning and theoretical analysis, it's important to note that:

They are not derived from large-scale, direct quantitative studies specifically measuring adverse events during the transport phase for each condition.
The weights represent a best-effort estimation to guide risk assessment and should be used in conjunction with clinical judgment and other patient-specific factors.
Contributing
Feedback and contributions to refine the weight values or expand the dictionary are welcome. Please refer to the theoretical_basis.txt document for the methodology used in the initial assignment.
