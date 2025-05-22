# 🚗 Car Evaluation Classifier – Flask + XGBoost

Este proyecto es una aplicación web construida con **Flask** que permite predecir la aceptabilidad de un carro (por ejemplo, `unacc`, `acc`, `good`, `vgood`) según sus características. El modelo fue entrenado con el dataset "Car Evaluation" de la UCI y desplegado en la nube usando **Render**.

---

## 🔗 Acceso al modelo

➡️ Puedes probar la aplicación aquí:  
📍 [https://flask-render-integration-fz95.onrender.com](https://flask-render-integration-fz95.onrender.com)

---

## 🧠 Modelo de Machine Learning

- Algoritmo: `XGBoostClassifier` (multiclase)
- Dataset: [Car Evaluation Data Set - UCI](https://archive.ics.uci.edu/ml/datasets/car+evaluation)
- Métricas:
  - F1 Macro Score: >0.98
  - AUC OvR: 1.00
- Preprocesamiento: `LabelEncoder` en variables categóricas

---

## 🖥 Estructura del proyecto

```
.
├── app.py                  # Servidor Flask
├── models/                 # Modelos y transformadores
│   ├── xgb_model.pkl
│   ├── label_encoders.pkl
│   └── feature_order.pkl
├── templates/
│   └── index.html          # Interfaz para introducir datos
├── requirements_deploy.txt
└── README.md
```

---

## 🧪 Cómo correrlo localmente

1. Clona este repositorio:
```bash
git clone https://github.com/4GeeksAcademy/efrainnalmeida-flask-render-integration.git
cd efrainnalmeida-flask-render-integration
```

2. Instala dependencias:
```bash
pip install -r requirements_deploy.txt
```

3. Ejecuta el servidor:
```bash
python app.py
```

Accede a [http://localhost:10000](http://localhost:10000)

---

## 🌐 Cómo fue desplegado

- Plataforma: [Render.com](https://render.com/)
- Servidor de producción: `gunicorn`
- Archivos clave: `requirements_deploy.txt` + `Procfile`

---

## 🧠 Autor

**Efraín Almeida**  
📘 [LinkedIn](https://www.linkedin.com/in/efrainnalmeida/)  
🎓 Proyecto desarrollado como parte de 4Geeks Academy
