# Fooling_HateBERT_XAI

To run this code:
1. use *python 3.9.6*.
2. (option a) `pip install -r requirements.txt` (gained from pip freeze > requirements.txt)
2. (option b) `pip install -r pip-requirements.txt` (gained from keeping track of installs)
2. (option c) in pip-requirements.txt comment the lines after the "manually added" comment. Save. Run `pip install -r pip-requirements.txt`. Install the last few commented packages manually with a pip install each.
3. download from https://osf.io/tbd58/files/osfstorage /HateBERT_fine_tuned_models/HateBERT_abuseval.zip
4. extract in ./HateBERT_fine_tuned_models/
    (extra info in the folder)
5. Open `Fooling_HateBERT_with_XAI.ipynb`
6. (optional) if you want to try the glove model, comment and uncomment according to the comment in `class perturb_word_shap()` init function in the Shap Perturbations section.


The notebook mostly has sections with function definitions. Everything needs to be run. At the end of the notebook is the `Running the Analysis` section. This is where all the functions defined are used for applying lime, shap and doing analysis on model predictions. Analysis is saved in `analysis_*.txt` files.

Intermediary data previously generated this way is saved in the `backup_generated_data` folder. New data is saved in the root project folder (cwd).