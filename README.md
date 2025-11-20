# Dog vs Cat Classification 🐶🐱

A deep learning project that classifies images of dogs and cats using **MobileNetV2** pre-trained model.

## Project Structure

```
DogVsCat/
└─ DogVsCat.ipynb      # Jupyter notebook with full training and evaluation
```

## Dataset

* Source: [Kaggle Dogs vs Cats](https://www.kaggle.com/competitions/dogs-vs-cats/data)
* Contains labeled images of dogs and cats.
* **Note:** Dataset is not included in the repo. You can download it using the Kaggle API (instructions below).

## Using Kaggle API to Download Dataset

1. Go to your Kaggle [Account](https://www.kaggle.com/) → **API** → **Create New API Token**.
   This will download a `kaggle.json` file containing your credentials.

2. In your notebook or terminal, configure the API:

```bash
# create Kaggle folder
!mkdir -p ~/.kaggle

# copy your kaggle.json to that folder
!cp kaggle.json ~/.kaggle/

# set permissions
!chmod 600 ~/.kaggle/kaggle.json
```

3. Download the Dogs vs Cats dataset:

```bash
!kaggle competitions download -c dogs-vs-cats
```

> ⚠️ Keep your `kaggle.json` private. Do **not** upload it to GitHub.

## How to Run

1. Open `DogVsCat.ipynb` in Jupyter Notebook.
2. Follow the notebook cells to preprocess data, train the model, and evaluate results.

## Requirements

* Python 3.x
* TensorFlow / Keras
* NumPy, Matplotlib

## License

MIT License

