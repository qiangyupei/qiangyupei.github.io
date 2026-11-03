---
layout: page
title: Bio
permalink: /bio/
main_nav: true
---

<div class="bio-container">
  <div class="bio-photo">
    <img src="{{ site.baseurl }}/assets/qiangyu.jpg" alt="Profile Picture">
  </div>

  <div class="bio-introduction">
    <p>
      I am a Senior Engineer at Huawei, working on reinforcement learning infrastructure and agent training systems. I earned my Ph.D. in Computer Architecture from Huazhong University of Science and Technology (HUST) in 2025, under the supervision of Prof. <a href="https://fangmingliu.github.io/" target="_blank" rel="noopener noreferrer">Fangming Liu</a>.
    </p>
    <p>
      My current work focuses on building <strong>efficient and scalable RL systems for LLMs and AI agents</strong>, with contributions to open-source projects such as <a href="https://github.com/verl-project/verl/tree/main" target="_blank" rel="noopener noreferrer">verl</a> and <a href="https://github.com/verl-project/uni-agent/tree/main" target="_blank" rel="noopener noreferrer">uni-agent</a>, spanning multi-agent and agentic RL training frameworks, post-training for kernel-generation agents, agent-aware scheduling of requests and KV cache blocks, and host and device memory optimization.
    </p>
  </div>
</div>

<h3>Education</h3>
<ul class="bio-list-style">
  <li><em>Sep 2019 – Jun 2025:</em>&nbsp; Ph.D. in Computer Architecture, Huazhong University of Science and Technology</li>
  <li><em>Sep 2015 – Jun 2019:</em>&nbsp; B.E. in Computer Science (Second Major), Huazhong University of Science and Technology</li>
  <li><em>Sep 2015 – Jun 2019:</em>&nbsp; B.S. in Physics (Major), Huazhong University of Science and Technology</li>
</ul>

<h3>Academic Services</h3>
<ul class="bio-list-style">
  <li>Artifact Evaluation Committee: OSDI (2022, 2023), SOSP (2023), ATC (2022, 2023)</li>
</ul>

<h3>Selected Open-Source Contributions</h3>
<ul class="bio-list-style">
  <li>
    <strong>Agentic RL &amp; Kernel Agents RL Training</strong>:
    Built on verl and uni-agent, this pipeline post-trains Qwen3.6-35B-A3B with GRPO for Ascend Triton kernel generation, using Claude Code as a black-box agent harness.
    <a href="https://github.com/verl-project/uni-agent/blob/main/examples/claude_code_kernel_task/README.md" target="_blank" rel="noopener noreferrer">Training Recipe</a>
    &middot; <a href="https://verl-project.github.io/posts/2026-09-23-uni-agent-v0-1-0/#recipes-and-experiments" target="_blank" rel="noopener noreferrer">Training Results</a>
  </li>
</ul>
