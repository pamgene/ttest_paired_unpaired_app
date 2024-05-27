# T-test paired on unpaired app

#### Description
Determines if there is a significant difference between the means of two groups. It performs Student's t-test on the data.

The input data should be log / VSN transformed.

<u> To run paired t-test: </u>  
- set Pairing factor in the wizard!

<u> To run unpaired t-test: </u>  
- leave Pairing factor empty in the wizard
- inside the app, in the t-test step / settings, set the setting for pairing to "unpaired"!

Leaving the pairing factor empty, but not setting the pairing parameter in the t-test operator / settings will lead to the error message: "Labels are required for a paired test."

#### The workflow has 2 operators:

- t_test_operator
- scale_operator
T_test operator settings:

detailed = True
var.equal = True
paired = False
reference level = 2 --> group with starting letter lower in the alphabet is the reference (control) group.

#### Views:

Volcano plot
Significant treatment effects (z-score scaled values)

