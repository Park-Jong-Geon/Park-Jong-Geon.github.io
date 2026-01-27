<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
.container {
  display: flex;
  margin: auto;
  gap: 40px;
}

.left {
  width: 30%;
}

.right {
  width: 70%;
}

.profile-img {
  width: 100%;
  border-radius: 0%;
  margin-bottom: 20px;
}

.contact {
  font-size: 0.95em;
  line-height: 2.4;
}


      
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
  .left, .right {
    width: 100%;
  }
}
</style>

<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<div class="container">

<div class="left">
<img id="profile-photo" src="assets/images/박종건_202511_1.jpg" class="profile-img" />

<div class="contact">
<i class="fa-solid fa-location-dot"></i> Republic of Korea <br>
<i class="fa-regular fa-envelope"></i> parkjonggeon@kaist.ac.kr <br>
<i class="fa-brands fa-github"></i> <a href="https://github.com/Park-Jong-Geon">GitHub</a> <br>
<i class="fa-brands fa-google-scholar"></i> <a href="https://scholar.google.com/citations?user=jKGjOb4AAAAJ">Google Scholar</a>
</div>

</div>



<div class="right">
<h2>About</h2>
<p style="font-size:0.85em">
Welcome, and thank you for visiting my homepage.<br>
<br>
I am currently a student at <span style="font-weight: 550;">CHA University Graduate School of Medicine</span>, with a strong academic interest in artificial intelligence and its applications in medicine. Prior to pursuing medical training, I received my master’s degree from <span style="font-weight: 550;">Kim Jaechul Graduate School of Artificial Intelligence at KAIST</span>, under the supervision of Professor <span style="font-weight: 550;">Juho Lee</span>, following a bachelor’s degree in Electrical Engineering, also from <span style="font-weight: 550;">KAIST</span>.<br>
<br>
During my master’s studies, I focused on generative models—particularly diffusion models and flow matching—with an emphasis on extending their applicability beyond image-based domains. Through this work, I developed a growing interest in AI-driven drug discovery and protein generation. These experiences ultimately shaped my broader vision of artificial intelligence as a transformative force in medicine and motivated my decision to pursue medical training.<br>
<br>
I believe, as many do, that the integration of artificial intelligence into clinical practice will fundamentally expand the boundaries of medicine in the near future. I hope to contribute to this ongoing transformation as a clinician-scientist. I welcome any discussions on medical AI research, interdisciplinary collaboration, and the future role of artificial intelligence in clinical medicine.
</p>

<h2>Publications</h2>

<p style="font-size:1em; margin: 0px 0px 0px 0px;">
Axial Neural Networks for Dimension-Free Foundation Models
</p>

<p style="font-size:0.8em; margin: 0px 0px 0px 0px;">
Hyunsu Kim, <strong>Jonggeon Park</strong>, Joan Bruna, Hongseok Yang, Juho Lee<br>
<em>The Thirty-ninth Annual Conference on Neural Information Processing Systems (NeurIPS)</em>, 2025 <br>

<a href="https://arxiv.org/pdf/2510.13665" target="_blank">[Paper]</a>
</p>

<hr>

<p style="font-size:1em; margin: 0px 0px 0px 0px;">
Ensemble Distribution Distillation via Flow Matching
</p>

<p style="font-size:0.8em; margin: 0px 0px 0px 0px;">
<strong>Jonggeon Park</strong><span class="eq-star">*</span>, Giung Nam<span class="eq-star">*</span>, Hyunsu Kim, Jongmin Yoon, Juho Lee<br>
<em>Forty-second International Conference on Machine Learning (ICML)</em>, 2025 <br>

<a href="https://openreview.net/pdf?id=waeJHU2oeI" target="_blank">[Paper]</a>

<a href="https://github.com/Park-Jong-Geon/EDFM" target="_blank">[GitHub]</a>
</p>

<hr>

<p style="font-size:1em; margin: 0px 0px 0px 0px;">
Stabilizing the training of consistency models with score guidance
</p>

<p style="font-size:0.8em; margin: 0px 0px 0px 0px;">
Jeongjun Lee<span class="eq-star">*</span>, <strong>Jonggeon Park</strong><span class="eq-star">*</span>, Jongmin Yoon, Juho Lee<br>
<em>ICML 2024 Workshop on Structured Probabilistic Inference & Generative Modeling</em>, 2024 <br>

<a href="https://openreview.net/pdf?id=6Q5828tzlp" target="_blank">[Paper]</a>

<a href="https://github.com/boingkiri/stabilizing_consistency" target="_blank">[GitHub]</a>
</p>

</div>

</div>

<script>
const photos = [
  "assets/images/박종건_202511_1.jpg",
  "assets/images/박종건_202511_2.jpg",
  "assets/images/박종건_202512.jpg",
];

const img = document.getElementById("profile-photo");
let lastSrc = img.src;

function changeImage() {
  let newSrc;
  do {
    const randomIndex = Math.floor(Math.random() * photos.length);
    newSrc = photos[randomIndex];
  } while (newSrc === lastSrc);
  
  img.src = newSrc;
  lastSrc = newSrc;
}

img.addEventListener("mouseenter", changeImage);
img.addEventListener("click", changeImage);
</script>
