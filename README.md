# BrainWaveClassifier-MEG-ML

The data consists of MEG recordings of a single subject, made during two separate measurement sessions (consecutive days). The task was to infer from one-second time windows the type of visual stimulus shown to the subject.The best submission of the 10 submissions, reached almost 70% accuracy.

In each session the subject was watching five different movie categories without audio. The goal is to predict the category of the movie the subject is watching The data was used in the MEG mind reading challenge organized in conjunction with the International Conference on Artificial Neural Networks (ICANN) 2011, sponsored by the PASCAL2 Challenge Programme.

Details, including information on the preprocessing, are here https://www.researchgate.net/publication/239918465_ICANNPASCAL2_Challenge_MEG_Mind_Reading_--_Overview_and_Results 

The five class values 

1. Artificial: screen saves.
2. Nature: clips from nature documentaries.
3. Foolball. Clips from La Lega.
4. Mr. Bean.
5. Chaplin.

Here’s a Notebook Overview:

1. Data Loading & Exploration: Import MEG signals and inspect shapes, statistics, and sample plots.
2. Train/Test Split: Create stratified splits to preserve class balance.
3. PCA & Classical Models: Reduce dimensionality; grid‑search KNN and SVM classifiers.
4. Statistical Classifier: Cross‑validated Naïve Bayes baseline with performance metrics.
5. Neural Network: Define, train, and regularize a PyTorch model; tune hyperparameters.
6. Results Visualization: Plot accuracy, loss curves, and compare model performances.
