## Replication Package
M. Macedo, Y. Tian, F. Cogo, and B. Adams, "Exploring the Impact of the Output Format on the Evaluation of Large Language Models for Code Translation," in Forge, 2024.

### Structure of the package

* Preliminary
* * ```original_dataset_before_processing.csv``` Base dataset with 4000 code samples.
* * ```dataset_after_processing.csv``` Dataset with 3,820 code samples with token lengths less than 3,072, includes the input code, test input and expected output. Please note that the input code does not contain ground truth (reference output code).

* RQ1
* * Contains the combined random sampled subsets for RQ1 (Vanilla and Reference Prompt subsets)
* RQ2
* * Contains the combined random sampled subsets for RQ2 (Vanilla and Control Prompt subsets)
* RQ3
* * ```inference_output_11_models_*``` Contains the inference output of the 11 models across the dataset used for each tested combination in RQ3 (CRE, VDE, VRE). Alongside the input code, translated code, test case input, expected test case output
* * ```rand_sample_350:``` The random samples to understand the compilation problems in RQ3
