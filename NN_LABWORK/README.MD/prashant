
# 📘 Road Condition Classifier Using LSTM (Accelerometer + Gyroscope)

## 🔍 Project Overview
This project builds an LSTM model that classifies road surface conditions based on 3-second segments of motion sensor data (accelerometer and gyroscope) from a two-wheeler ride.

## 📱 Android App
A custom Android app collects sensor data (`accel_x/y/z`, `gyro_x/y/z`) while riding on various surfaces:
- Kankar Road
- Bitumen Road
- Concrete Road
- Single Speed Breaker
- Multiple Speed Breakers

## 📊 Dataset
- Sensor readings are recorded at 50 Hz (50 readings per second).
- Each 3-second sample → 150 time steps.
- Label encoded for 5 classes.

## 🧠 Model
- LSTM Neural Network using Keras/TensorFlow.
- Input Shape: `(150, 6)` → 150 time steps, 6 features.
- Output: Softmax classification (5 classes).
- Uses:
  - `StandardScaler` for normalization.
  - `LabelEncoder` for categorical labels.
  - `EarlyStopping` + `ModelCheckpoint` for optimal training.

## ✅ Accuracy
- Achieved over **80%+ accuracy**, and further improvements with:
  - Dropout regularization
  - Additional LSTM units
  - Data augmentation (future)

## 💾 Files Saved
- `road_condition_model.keras`: Final trained model.
- `best_model.keras`: Best model (saved during training).
- `road_condition_dataset.csv`: Your preprocessed dataset.

## 🚀 Bonus Feature (Future Scope)
Use the trained model to:
- Detect **rash driving** (based on sudden jerks, abnormal gyro patterns).
- Integrate alerts in the Android app in real time.
