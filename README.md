# :computer: Port Scan Detection using ML
---

<i>Bu çalışma, aiseclab.org bünyesinde <b>cyber-bot</b> ekibi projesi olarak geliştirilmiştir.</i>

# :computer: Amaç
---

* Makine öğrenmesi modellerini kullarak port taraması sonuçları zararlı ve zararsız olarak sınıflandırılacaktır. Kullanılan veri setine ulaşmak için [bu bağlantıya](https://www.kaggle.com/datasets/merfarukdilbaz/probingportscandataset) tıklayabilirsiniz.
<br/>

# :computer: Ekip Üyeleri
---
**Danışman**: [Atakan AK](https://github.com/Kuroin)
<br/>

1. [Doğukan ESEN](https://github.com/DogukanEsen)
2. [İrem USLU](https://github.com/irem6142)
3. [Esmanur HURMA](https://github.com/esmanurhurma)
4. [Ömer Faruk DİLBAZ](https://github.com/OmerFarukDilbaz)
<br/>

# :computer: Gerekli Kütüphaneler

* Kullanılan kütüphaneler ve versiyon bilgileri aşağıda belirtilmiştir.

```shell
blinker==1.6.2
click==8.1.7
colorama==0.4.6
Flask==2.2.5
Flask-Cors==4.0.0
gunicorn==21.2.0
importlib-metadata==6.7.0
itsdangerous==2.1.2
Jinja2==3.1.2
joblib==1.3.2
MarkupSafe==2.1.3
numpy==1.24.4
packaging==23.1
patsy==0.5.3
plotly==5.17.0
plotly-express==0.4.1
python-dateutil==2.8.2
pytz==2023.3.post1
scikit-learn==1.3.1
scipy==1.11.3
six==1.16.0
statsmodels==0.14.0
tenacity==8.2.3
threadpoolctl==3.2.0
tzdata==2023.3
Werkzeug==2.3.7
zipp==3.17.0

```
<br/>

# :computer: Kurulum
---

* Gerekli paketleri kurduktan sonra uygulamayı kullanmaya başlayabilirsiniz. Kurulum yapmadan [bu link](https://ml-port-scanner.netlify.app) üzerinden modeli test edebilirsiniz.

```python3
pip install -r requirements.txt
# Ana uygulamayı çalıştırmak için
cd backend
python3 app.py
```
<br/>

# :computer: Modeller
---

* Problemi çözmek için DecisionTree ve SVC modelleri kullanılmıştır. Kullanılan modellere ait veriler aşağıda belirtilmiştir.

| Model | Train Accuracy | Test Accuracy | F1-Score | Precision Score | Recall Score |
| ----- | -------------- | ------------- | -------- | --------------- | ------------ |
| DecisionTreeClassifier | 0.9968 | 0.9974 | 0.9973 | 0.9974 | 0.9974 | 
| SVC | X | 0.8153 | 0.7899 | 0.8504 | 0.8153 | 
