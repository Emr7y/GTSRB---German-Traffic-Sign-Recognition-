# GTSRB Verkehrszeichenerkennung \U0001F6A6

Dieses Projekt nutzt ein Convolutional Neural Network (CNN), um Verkehrszeichen aus dem deutschen GTSRB-Datensatz zu klassifizieren. Es wurde mit TensorFlow/Keras trainiert und als Streamlit-App zur Interaktion umgesetzt.

---

## ✨ Demo



---

## ⚡ Projekt-Features

- \U0001F4C2 Datensatz: [GTSRB - German Traffic Sign Recognition Benchmark](https://www.kaggle.com/datasets/dk58554/gtsrb-german-traffic-sign)
- \U0001F9EE Modell: CNN mit regulärer Dropout- und L1/L2-Regularisierung
- \U0001F4F7 Bild-Upload zur Vorhersage von Verkehrszeichen
- ⚖ Anzeige der Modell-Sicherheit in Prozent
- \U0001F5FA️ Vorhersage des konkreten Schildtyps
- ✨ Streamlit-Web-App mit deutscher UI

---

## \U0001F527 Setup

```bash
# 1. Repository klonen
git clone https://github.com/deinname/gtsrb-traffic-sign-app.git
cd gtsrb-traffic-sign-app

# 2. Virtuelle Umgebung (optional)
python -m venv venv
source venv/bin/activate  # oder .\venv\Scripts\activate auf Windows

# 3. Abhängigkeiten installieren
pip install -r requirements.txt

# 4. App starten
streamlit run app.py
```

---

## \U0001F50E Modellarchitektur (Kurzfassung)

```python
Conv2D → BatchNorm → Conv2D → BatchNorm → ...
Flatten → Dense(1024) → Dropout → Dense(256) → Output(43 Klassen)
```

---

## \U0001F4DD Beispiel: Vorhersage

```python
predictImage("Test/01250.png")
# Output: 'No passing veh over 3.5 tons (97.23% confidence)'
```

---

## \U0001F4CB Dateiübersicht

```
├── app.py                  # Streamlit-App
├── gtsrb_model.keras       # Trainiertes Modell
├── requirements.txt        # Python-Abhängigkeiten
├── README.md               # Diese Datei :)
├── demo_screenshot.png     # Screenshot der Anwendung
└── Test/                   # Beispiel-Testbilder
```

---

## ❤️ Dank & Quelle

Made with ❤️ by **Emr7y**\
Modell: CNN\
Datenquelle: [Kaggle GTSRB Dataset](https://www.kaggle.com/datasets/dk58554/gtsrb-german-traffic-sign)

---

## \U0001F680 Hugging Face / GitHub Deployment

> Hinweis: Bild-Upload funktioniert **nicht direkt auf Hugging Face**, daher wird ein GitHub-Link bevorzugt.

---

