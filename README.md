<!-- README.html (Use directly in README.md) -->
<div align="center">
  <h1>🥦 VegQual: A Quality-Based Vegetable Image Dataset for Defect Detection Using YOLO Models</h1>

  <p>
    <a href="#"><img src="https://img.shields.io/badge/Paper-Link-blue?style=flat-square" alt="Paper"></a>
    <a href="#"><img src="https://img.shields.io/badge/Dataset-Download-green?style=flat-square" alt="Dataset"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License"></a>
  </p>
</div>

<hr>

<style>
  .section { margin: 1.5rem 0; }
  .kicker { font-size: 0.95rem; color: #555; }
  h2 { margin-top: 1.4rem; }
  h3 { margin-top: 1rem; }
  .pill {
    display: inline-block;
    background: #f6f8fa;
    border: 1px solid #eaecef;
    border-radius: 999px;
    padding: 0.25rem 0.75rem;
    margin: 0.2rem 0.2rem 0 0;
    font-size: 0.9rem;
  }
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 0.75rem 0;
  }
  th, td {
    border: 1px solid #dfe2e5;
    padding: 0.55rem 0.6rem;
  }
  th {
    background: #ffd89e;
  }
  tbody tr:nth-child(odd) { background: #fff; }
  tbody tr:nth-child(even) { background: #fafbfc; }
  code, pre code {
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", monospace;
  }
  pre {
    background: #0b1021;
    color: #e6edf3;
    padding: 1rem;
    border-radius: 8px;
    overflow: auto;
    border: 1px solid #111728;
  }
  .hr {
    height: 1px;
    background: #e5e7eb;
    border: 0;
    margin: 1.5rem 0;
  }
  .center { text-align: center; }
  .badgebar a img { margin: 0.25rem; }
</style>

<div class="section" id="overview">
  <h2>🌱 Overview</h2>

  <p><strong>VegQual</strong> is a specialized multiclass image dataset designed for
  <strong>real-time classification and defect detection of vegetables</strong>.
  The dataset contains images of both <strong>fresh</strong> and <strong>defective</strong> samples across
  <strong>seven vegetable types</strong>, collected under diverse environmental and lighting conditions to
  support robust training and generalization.</p>

  <p class="kicker">This dataset supports computer vision research focused on:</p>
  <div>
    <span class="pill">Quality assessment of agricultural produce</span>
    <span class="pill">Real-time defect detection systems</span>
    <span class="pill">YOLO-based object detection training & evaluation</span>
  </div>

  <p>Each image in VegQual is annotated using the <strong>YOLO format</strong>, with bounding boxes that
  clearly identify fresh and defective instances. VegQual aims to help researchers, students, and practitioners
  build AI-driven solutions for improving agricultural quality inspection and reducing food waste.</p>

  <h3>🧩 Key Highlights</h3>
  <ul>
    <li><strong>7 vegetables, 14 classes</strong> (fresh & defective for each): Tomato, Potato, Bitter Gourd, Pointed Gourd, Onion, Capsicum, and Brinjal</li>
    <li><strong>4,736 annotated images</strong> (2,386 defective + 2,350 fresh)</li>
    <li><strong>High-quality YOLO annotations</strong></li>
    <li><strong>Benchmark results</strong> for YOLOv9 and YOLOv11</li>
    <li>Ideal for <em>machine learning, agriculture automation, and quality inspection systems</em></li>
  </ul>
</div>

<hr class="hr">

<div class="section" id="dataset-summary">
  <h2>📊 Dataset Summary</h2>

  <table>
    <thead>
      <tr>
        <th>Vegetable Name</th>
        <th>Defective Images</th>
        <th>Fresh Images</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Tomato</td><td align="right">190</td><td align="right">167</td></tr>
      <tr><td>Potato</td><td align="right">105</td><td align="right">442</td></tr>
      <tr><td>Bitter Gourd</td><td align="right">629</td><td align="right">413</td></tr>
      <tr><td>Pointed Gourd</td><td align="right">256</td><td align="right">175</td></tr>
      <tr><td>Onion</td><td align="right">518</td><td align="right">245</td></tr>
      <tr><td>Capsicum</td><td align="right">295</td><td align="right">569</td></tr>
      <tr><td>Brinjal</td><td align="right">393</td><td align="right">339</td></tr>
      <tr>
        <th>Total</th>
        <th align="right">2,386</th>
        <th align="right">2,350</th>
      </tr>
    </tbody>
  </table>

  <p><strong>Total Images:</strong> 4,736 &nbsp; • &nbsp; <strong>Number of Classes:</strong> 14 &nbsp; • &nbsp; <strong>Annotations:</strong> YOLO (bounding boxes)</p>
</div>

<hr class="hr">

<div class="section" id="performance">
  <h2>⚙️ Model Performance</h2>

  <table>
    <thead>
      <tr>
        <th>Model</th>
        <th>Precision (%)</th>
        <th>Recall (%)</th>
        <th>PR (%)</th>
        <th>F1-score (%)</th>
        <th>mAP@50 (%)</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>YOLOv9</td><td align="right">89.4</td><td align="right">92.6</td><td align="right">94.3</td><td align="right">90.8</td><td align="right">94.3</td></tr>
      <tr><td>YOLOv11</td><td align="right">89.8</td><td align="right">89.2</td><td align="right">93.9</td><td align="right">89.4</td><td align="right">93.9</td></tr>
    </tbody>
  </table>
</div>

<hr class="hr">

<div class="section" id="methodology">
  <h2>🧠 Methodology</h2>
  <ol>
    <li><strong>Image Acquisition:</strong> Captured using multiple smartphone cameras under daylight and indoor lighting.</li>
    <li><strong>Annotation:</strong> Bounding boxes labeled manually following the YOLO format.</li>
    <li><strong>Model Training:</strong> YOLOv9 and YOLOv11 trained for comparative analysis.</li>
    <li><strong>Evaluation:</strong> Precision, Recall, F1-score, and mAP@50.</li>
  </ol>
</div>

<hr class="hr">

<div class="section" id="contribution">
  <h2>🧩 Contribution</h2>

  <p><strong>Authors:</strong><br>
  Tarek Rahman¹, Md Rahadul Islam Jishan¹, Robiul Islam¹, Md Rakibul Islam¹, and Jannatul Tajrian¹</p>

  <p><strong>Supervisor:</strong><br>
  Ohidujjaman¹*</p>

  <p>¹ Department of Computer Science and Engineering<br>
  *Corresponding author and project supervisor</p>
</div>

<hr class="hr">

<div class="section" id="how-to-use">
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

<hr class="hr">

<div class="section center" id="contact">
  <h2>📬 Contact</h2>

  <p><strong>Tarek Rahman</strong></p>

  <p class="badgebar">
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

<hr class="hr">

<div class="section" id="citation">
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
