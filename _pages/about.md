---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

My name is Yue HUANG. I am currently a PhD student of <a href="https://tint-research.com/index">TINT</a>, supervised by <a href="https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page?id=574">Prof. Huayi Duan</a> at <a href="https://www.hkust-gz.edu.cn/">HKUST(GZ)</a>. Prior to that, I earned my MPhil degree from HKUST<sup id="fnref-hkust"><a href="#fn-hkust">[1]</a></sup> under the guidance of <a href="https://sites.google.com/view/jtang">Prof. Jing TANG</a> in October 2025.

<div class="notice--info" markdown="1">
**Research Interests:**
- Agent and Internet Security
- Blockchain Security
- Formal Method

If you are interested in collaboration or potential research opportunities, feel free to reach out!
</div>

# 🔥 News
- *2025.08*: &nbsp;📌📌 Released our paper [TraceLLM: Security Diagnosis Through Traces and Smart Contracts in Ethereum](https://arxiv.org/abs/2509.03037).
- *2025.07*: &nbsp;📌📌 Released our paper [The Price of Cheaper Data: Measuring the Strategic Inefficiencies in the Post-EIP-4844 Ethereum Market](https://arxiv.org/pdf/2411.03892).
- *2025.02*: &nbsp;📌📌 Our paper [Private Order Flows and Builder Bidding Dynamics: The Road to Monopoly in Ethereum’s Block Building Market](https://dl.acm.org/doi/pdf/10.1145/3696410.3714754) was accepted by WWW 2025.

<span class='anchor' id='publications'></span>
# 📝 Publications
(# represents the corresponding author of each paper.)
1. Shuzheng Wang, **Yue HUANG**, Zhuoer Xu, Yuming Huang, and Jing TANG#. TraceLLM: Security Diagnosis Through Traces and Smart Contracts in Ethereum. arXiv.
2. **Yue HUANG**, Shuzheng Wang, Yuming Huang, Gareth Tyson, and Jing TANG#. The Price of Cheaper Data: Measuring the Strategic Inefficiencies in the Post-EIP-4844 Ethereum Market. arXiv.
3. Shuzheng Wang, **Yue HUANG**, Wenqin Zhang, Yuming Huang, Xuechao Wang, and Jing TANG#. Private Order Flows and Builder Bidding Dynamics: The Road to Monopoly in Ethereum’s Block Building Market. WWW 2025.
4. Jiande Huang, **Yue HUANG**, SG Hassan, Longqin Xu, and Shuangyin Liu#. Dissolved Oxygen Content Interval Prediction based on Auto Regression Recurrent Neural Network. Journal of Ambient Intelligence and Humanized Computing 14 (6), 7255-7264, 2021.


<span class='anchor' id='honors'></span>
# 🎖 Honors and Awards
<ul id="honors-list">
  <li><em>2026.01</em> PostGraduate Scholarship (15,000 CNY per Month).</li>
  <li><em>2024.09</em> PostGraduate Scholarship (10,000 CNY per Month).</li>
  <li><em>2023.09</em> PostGraduate Scholarship (10,000 CNY per Month).</li>
  <li><em>2023.05</em> First-class Scholarship (1/216).</li>
  <li><em>2022.10</em> <strong><font color="red">National Scholarship</font></strong> (Top 0.2%, Awarded by the <a href="http://en.moe.gov.cn/">Ministry of Education of China</a>).</li>
  <li><em>2022.10</em> Special-class Scholarship (Top 0.05%, 10/20224).</li>
  <li><em>2021.06</em> First Prize of China College Student Computing Contest.</li>
  <li><em>2021.06</em> First Prize of "Huazi Cup" Guangdong University Students' Computer Works Competition.</li>
  <li><em>2021.05</em> Third Prize in the Guangdong-Hong Kong-Macao Greater Bay Area IT System Development Competition.</li>
  <li><em>2021.04</em> Third Prize of the 16th "Challenge Cup" Guangdong University Students' Extra-curricular Academic Science and Technology Works Competition.</li>
  <li><em>2021.09</em>, <em>2020.09</em> Twice Merit Students, Twice <strong>National</strong> Inspiration Scholarships.</li>
</ul>

<style>
  #honors-toggle {
    display: none;
    margin-top: 0.6em;
    padding: 0.38em 0.82em;
    border: 1px solid #d0d7de;
    border-radius: 999px;
    background: #f7f9fc;
    color: #374151;
    font-size: 0.88em;
    font-weight: 600;
    line-height: 1.2;
    cursor: pointer;
    transition: all 0.2s ease;
  }

  #honors-toggle:hover {
    background: #eef3ff;
    border-color: #b7c5e3;
    color: #1f3d7a;
  }

  #honors-toggle .toggle-icon {
    display: inline-block;
    margin-right: 0.45em;
    font-family: monospace;
    transform-origin: center;
    transition: transform 0.2s ease;
  }

  #honors-toggle.expanded .toggle-icon {
    transform: rotate(90deg);
  }
</style>

<button id="honors-toggle" type="button">
  <span class="toggle-icon" aria-hidden="true">&gt;</span>
  <span class="toggle-label">Show more</span>
</button>

<script>
  (function () {
    var maxVisible = 5;
    var list = document.getElementById("honors-list");
    var toggle = document.getElementById("honors-toggle");
    if (!list || !toggle) return;

    var items = list.querySelectorAll("li");
    if (items.length <= maxVisible) return;

    var expanded = false;
    var label = toggle.querySelector(".toggle-label");
    function render() {
      for (var i = 0; i < items.length; i++) {
        items[i].style.display = expanded || i < maxVisible ? "list-item" : "none";
      }
      if (label) {
        label.textContent = expanded ? "Show less" : "Show more";
      }
      toggle.classList.toggle("expanded", expanded);
    }

    toggle.style.display = "inline-block";
    render();
    toggle.addEventListener("click", function () {
      expanded = !expanded;
      render();
    });
  })();
</script>


# 📖 Educations
- *2026.01 - present*, PhD in Data Science and Analytics, Information Hub, The Hong Kong University of Science and Technology (Guangzhou).
- *2023.09 - 2025.10*, MPhil in Data Science and Analytics, Information Hub, The Hong Kong University of Science and Technology (Guangzhou).
- *2019.09 - 2023.06*, B.Eng. in Computer Science and Technology, School of Information Science and Technology, Zhongkai University of Agriculture and Engineering, Guangzhou, China.


# 💻 Experiences
- *2025.09 - 2026.01*, Research Assistant at HKUST (GZ), Guangzhou, China.
- *2022.11 - 2023.08*, Research Assistant at HKUST (GZ), Guangzhou, China.
- *2019.12 - 2022.10*, Front-end & Back-end Intern at Guangdong Smart Agriculture Engineering Technology Research Center, Guangzhou, China.

<span class='anchor' id='services'></span>
# 📜 Services
- Reviewer for ACM Web Conference (WWW): 2024, 2025
- Student Volunteer for VLDB 2024
- Teaching Assistant of HKUST (GZ) DSAA 5020 Foundations of Data Science

<p id="fn-hkust" style="font-size: 13px;"><sup>[1]</sup> I completed my MPhil study at the Guangzhou campus, rather than the Clear Water Bay campus.<a href="#fnref-hkust">↩</a></p>