<h1>🚀 Big Data Cybersecurity Threat Detection</h1>

<p>A real-time cybersecurity platform using Big Data and Machine Learning to detect and analyze security threats in network traffic. Processes streaming data through distributed architecture to identify DDoS attacks, malware, phishing, and ransomware with high accuracy.</p>

---

<h2>📑 Table of Contents</h2>
<ul>
  <li><a href="#overview">🎯 Project Overview</a></li>
  <li><a href="#architecture">🏗️ Architecture</a></li>
  <li><a href="#tech-stack">⚙️ Technology Stack</a></li>
  <li><a href="#components">📂 Project Components</a></li>
  <li><a href="#getting-started">🚀 Getting Started</a></li>
  <li><a href="#results">📊 Results</a></li>
  <li><a href="#screenshots">📸 Screenshots</a></li>
  <li><a href="#author">👨‍💻 Author</a></li>
</ul>

---

<h2 id="overview">🎯 Project Overview</h2>
<p><b>Goal</b>: Detect anomalies and predict potential cyber threats (DDoS, malware, phishing, ransomware) from network traffic logs in real-time.</p>
<p><b>Approach</b>:</p>
<ul>
  <li>Generate synthetic network logs</li>
  <li>Stream logs via <b>Apache Kafka</b></li>
  <li>Process with <b>Apache Spark Streaming</b></li>
  <li>Apply trained <b>ML model</b> for threat classification</li>
  <li>Store results in <b>InfluxDB</b></li>
  <li>Visualize anomalies and traffic in <b>Grafana</b></li>
</ul>

---

<h2 id="architecture">🏗️ Architecture</h2>
<p><img src="./screenshots/architecture-diagram.png" alt="System Architecture" width="700"/></p>
<p><i>Complete pipeline architecture showing data flow from log generation to visualization: [Log Generator] → [Kafka Producer] → [Kafka Topic: logs] → [Spark Streaming + ML Model] → [InfluxDB] → [Grafana Dashboard]</i></p>

---

<h2 id="tech-stack">⚙️ Technology Stack</h2>
<ul>
  <li><b>Docker Compose</b> – Service orchestration</li>
  <li><b>Apache Kafka</b> – Data ingestion</li>
  <li><b>Apache Spark Streaming</b> – Real-time data processing</li>
  <li><b>Scikit-learn</b> – Machine Learning (Logistic Regression - F1 = 0.77)</li>
  <li><b>InfluxDB</b> – Time-series database</li>
  <li><b>Grafana</b> – Interactive visualization</li>
  <li><b>Jupyter Notebooks</b> – Development & experimentation</li>
</ul>

---

<h2 id="components">📂 Project Components</h2>
<ul>
  <li><a href="./notebooks/generator.ipynb">notebooks/generator.ipynb</a> → Generates synthetic network logs</li>
  <li><a href="./notebooks/kafka_producer.ipynb">notebooks/kafka_producer.ipynb</a> → Sends logs to Kafka topic</li>
  <li><a href="./notebooks/train_threat_classifier.ipynb">notebooks/train_threat_classifier.ipynb</a> → Trains ML models</li>
  <li><a href="./notebooks/spark_processing.ipynb">notebooks/spark_processing.ipynb</a> → Full processing pipeline</li>
  <li><a href="./docker-compose.yml">docker-compose.yml</a> → Service orchestration</li>
</ul>

---

<h2 id="getting-started">🚀 Getting Started</h2>
<ol>
  <li><b>Start Infrastructure:</b> <code>docker compose up -d</code></li>
  <li><b>Generate Logs:</b> Run generator notebook</li>
  <li><b>Send to Kafka:</b> Run producer notebook</li>
  <li><b>Process Data:</b> Run Spark streaming notebook</li>
  <li><b>Visualize:</b> Access Grafana at http://localhost:3000</li>
</ol>

---

<h2 id="results">📊 Results</h2>
<p><b>Machine Learning Performance:</b></p>
<ul>
  <li>Best Model: <b>Logistic Regression</b></li>
  <li>F1 Score: <b>0.77</b></li>
</ul>
<p><b>Grafana Dashboards:</b></p>
<ul>
  <li>Real-time anomaly detection</li>
  <li>Top malicious IPs</li>
  <li>Geographic threat map</li>
  <li>Protocol monitoring</li>
</ul>

---

<h2 id="screenshots">📸 Screenshots</h2>

<h3>🔹 Grafana Dashboards</h3>

<h4>Network Traffic Analysis</h4>
<p><img src="./screenshots/grafana-traffic.png" alt="Traffic Dashboard" width="700"/></p>
<p><i>Real-time network traffic volume and protocol monitoring</i></p>

<h4>Real-time Threat Detection</h4>
<p><img src="./screenshots/grafana-threat-detection.png" alt="Threat Detection Dashboard" width="700"/></p>
<p><i>Live monitoring of cybersecurity threats and anomalies</i></p>

<h4>Geographic Threat Map</h4>
<p><img src="./screenshots/grafana-geographic.png" alt="Geographic Dashboard" width="700"/></p>
<p><i>Geographic visualization of threat origins and distribution</i></p>

---

<h2 id="author">👨‍💻 Author</h2>
<ul>
  <li><b>Fahd El Attar</b></li>
</ul>
