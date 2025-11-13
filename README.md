<!-- VegQual README (GitHub-Compatible HTML Version) -->
<div align="center">
  <h1>🥦 VegQual: A Multiclass Dataset for Real-Time Detection of Fresh and Defective Vegetables Using Deep Learning</h1>

  <p>
    <a href="#"><img src="https://img.shields.io/badge/Paper-Link-blue?style=flat-square" alt="Paper"></a>
    <a href="#"><img src="https://img.shields.io/badge/Dataset-Download-green?style=flat-square" alt="Dataset"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License"></a>
  </p>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2 style="color:#1E8449;">🌱 Overview</h2>
  <p><strong>VegQual</strong> is a specialized multiclass image dataset designed for
  <strong>real-time classification and defect detection of vegetables</strong>.
  The dataset contains images of both <strong>fresh</strong> and <strong>defective</strong> samples across
  <strong>seven vegetable types</strong>, collected under diverse environmental and lighting conditions to
  support robust training and generalization.</p>

  <p>This dataset supports computer vision research focused on:</p>
  <ul>
    <li>Quality assessment of agricultural produce</li>
    <li>Real-time defect detection systems</li>
    <li>Training and evaluation of <strong>YOLO-based object detection models</strong></li>
  </ul>

  <p>Each image in VegQual is annotated using the <strong>YOLO format</strong>, with bounding boxes that
  clearly identify fresh and defective instances. VegQual aims to help researchers, students, and practitioners
  build AI-driven solutions for improving agricultural quality inspection and reducing food waste.</p>

  <h3 style="color:#F39C12;">🧩 Key Highlights</h3>
  <ul>
    <li><strong>7 vegetables, 14 classes</strong> (fresh & defective): Tomato, Potato, Bitter Gourd, Pointed Gourd, Onion, Capsicum, Brinjal</li>
    <li><strong>4,736 annotated images</strong> (2,386 defective + 2,350 fresh)</li>
    <li><strong>High-quality YOLO annotations</strong></li>
    <li><strong>Benchmark results</strong> for YOLOv9 and YOLOv11</li>
    <li>Ideal for <em>machine learning, agriculture automation, and quality inspection systems</em></li>
  </ul>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>📊 Dataset Summary</h2>

  <table style="width:100%; border-collapse:collapse;">
    <thead>
      <tr style="background:#ffd89e;">
        <th style="border:1px solid #ccc; padding:8px;">Vegetable Name</th>
        <th style="border:1px solid #ccc; padding:8px;">Defective Images</th>
        <th style="border:1px solid #ccc; padding:8px;">Fresh Images</th>
      </tr>
    </thead>
    <tbody>
      <tr><td style="border:1px solid #ccc; padding:6px;">Tomato</td><td align="right">190</td><td align="right">167</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Potato</td><td align="right">105</td><td align="right">442</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Bitter Gourd</td><td align="right">629</td><td align="right">413</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Pointed Gourd</td><td align="right">256</td><td align="right">175</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Onion</td><td align="right">518</td><td align="right">245</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Capsicum</td><td align="right">295</td><td align="right">569</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Brinjal</td><td align="right">393</td><td align="right">339</td></tr>
      <tr style="background:#fff3cd;">
        <th>Total</th><th align="right">2,386</th><th align="right">2,350</th>
      </tr>
    </tbody>
  </table>

  <p><strong>Total Images:</strong> 4,736 &nbsp; | &nbsp; <strong>Number of Classes:</strong> 14 &nbsp; | &nbsp; <strong>Annotations:</strong> YOLO format</p>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>⚙️ Model Performance</h2>
  <table style="width:100%; border-collapse:collapse;">
    <thead>
      <tr style="background:#ffd89e;">
        <th style="border:1px solid #ccc; padding:8px;">Model</th>
        <th style="border:1px solid #ccc; padding:8px;">Precision (%)</th>
        <th style="border:1px solid #ccc; padding:8px;">Recall (%)</th>
        <th style="border:1px solid #ccc; padding:8px;">PR (%)</th>
        <th style="border:1px solid #ccc; padding:8px;">F1-score (%)</th>
        <th style="border:1px solid #ccc; padding:8px;">mAP@50 (%)</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>YOLOv9</td><td align="right">88.7</td><td align="right">92.6</td><td align="right">93.2</td><td align="right">90.6</td><td align="right">93.2</td></tr>
      <tr><td>YOLOv11</td><td align="right">88</td><td align="right">90.5</td><td align="right">94.3</td><td align="right">89.23</td><td align="right">94.3</td></tr>
    </tbody>
  </table>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>🧠 Methodology</h2>
  <ol>
    <li><strong>Image Acquisition:</strong> Captured using multiple smartphone cameras under daylight and indoor lighting.</li>
    <li><strong>Annotation:</strong> Bounding boxes labeled manually following the YOLO format.</li>
    <li><strong>Model Training:</strong> YOLOv9 and YOLOv11 trained for comparative analysis.</li>
    <li><strong>Evaluation:</strong> Precision, Recall, F1-score, and mAP@50.</li>
  </ol>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>🧩 Contribution</h2>
  <p><strong>Authors:</strong><br>
  Tarek Rahman¹, Md Rahadul Islam Jishan¹, Robiul Islam¹, Md Rakibul Islam¹, and Jannatul Tajrian¹</p>

  <p><strong>Supervisor:</strong><br>
  Ohidujjaman¹*</p>

  <p>¹ Department of Computer Science and Engineering<br>
  *Corresponding author and project supervisor</p>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>💻 How to Use</h2>
  <pre><code># Clone this repository
git clone https://github.com/yourusername/VegQual.git

# Navigate into the directory
cd VegQual

# Install dependencies
pip install -r requirements.txt

# Train YOLO model
python train.py --data vegqual.yaml --weights yolov9.pt

# Evaluate the model
python test.py --weights runs/train/weights/best.pt --data vegqual.yaml
</code></pre>
</div>

<hr>

<div align="center" style="margin: 1.5rem 0;">
  <h2>📬 Contact</h2>
  <p><strong>Tarek Rahman</strong></p>

  <p>
    <a href="mailto:tarekrahamn01@gmail.com?subject=VegQual%20Inquiry">
      <img src="https://img.shields.io/badge/Email-tarekrahamn01%40gmail.com-red?logo=gmail&logoColor=white&style=for-the-badge" alt="Email">
    </a>
    <a href="https://www.linkedin.com/in/tarek-rahmantr">
      <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin&logoColor=white&style=for-the-badge" alt="LinkedIn">
    </a>
    <a href="https://scholar.google.com/citations?user=n_PyeXwAAAAJ&hl=en">
      <img src="https://img.shields.io/badge/Google%20Scholar-Profile-4285F4?logo=googlescholar&logoColor=white&style=for-the-badge" alt="Google Scholar">
    </a>
  </p>
</div>

<hr>

<div style="margin: 1.5rem 0;">
  <h2>📜 Citation</h2>
  <p>If you use this dataset or code in your research, please cite:</p>

  <pre><code>@misc{rahman2025vegqual,
  author       = {Rahman, T. and Jishan, Md Rahadul Islam and Islam, Robiul and Islam, Md Rakibul and Tajrian, Jannatul},
  title        = {A Multiclass Dataset for Real-Time Fresh and Defective Vegetables},
  year         = {2025},
  month        = nov,
  publisher    = {Figshare},
  url          = {https://figshare.com/articles/dataset/_/30596084/0}
}
</code></pre>
</div>
