## Installation

```bash
cd cs4025code
```

```bash
python3 -m venv cs4025code-env
```

```bash
source cs4025code-env/bin/activate
```

```bash
pip install -r requirements.txt
```

```bash
python3 -m spacy download en
```

```bash
python3 -m spacy download en_core_web_lg
```

```bash
python3 -m nltk.downloader all
```

## Usage

To train a new classifier and print its accuracy, run:
```bash
python3 main.py
```

To save the classifier into a file called saved_classifier.pickle, run:
```bash
python3 main.py --save
```

To load the saved classifier and print its accuracy, run:
```bash
python3 main.py --load
```

To load the saved classifier and print the confusion matrix of the test set, run:

```bash
python3 main.py --cm
```

To save the preprocessed data sets to enable fast classifier training (python3 main.py --fast), run:

```bash
python3 main.py --preprocess
```

To use saved preprocessed data sets and train new classifier then print its accuracy, run:

```bash
python3 main.py --fast
```