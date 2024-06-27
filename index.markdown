---
layout: mydefault
---

<html>

<head>
  <meta charset="utf-8">
  <meta name="description" content="IInfiBench: Evaluating the Question-Answering Capabilities of Code LLMs">
  <meta name="keywords" content="InfiCoder-Eval, code-generation, large-language-model, benchmark">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>InfiBench: Evaluating the Question-Answering Capabilities of Code LLMs</title>

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

  <link rel="stylesheet" href="./static/css/bulma.min.css">
  <link rel="stylesheet" href="./static/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="./static/css/bulma-slider.min.css">
  <link rel="stylesheet" href="./static/css/fontawesome.all.min.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="./static/css/index.css">

  <link rel="stylesheet" href="./bower_components/bootstrap/dist/css/bootstrap.table.min.css">
  <!--  <link rel="stylesheet" href="bower_components/bootstrap/dist/css/bootstrap.min.css">-->
  <link rel="stylesheet" href="./stylesheets/layout.css">
  <link rel="stylesheet" href="./stylesheets/index.css">

  <!-- for print the table -->
  <script type="text/javascript" charset="utf8" src="https://code.jquery.com/jquery-3.6.0.slim.min.js"></script>

  <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.11.3/css/jquery.dataTables.css">
  <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.11.3/js/jquery.dataTables.js"></script>

  <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.11.3/css/dataTables.bootstrap5.min.css">
  <script src="https://cdn.datatables.net/1.11.3/js/dataTables.bootstrap5.min.js"></script>

  <link rel="icon" href="./static/images/inficoder_eval_logo2.png">

  <script defer src="./static/js/fontawesome.all.min.js"></script>
  <script src="./static/js/bulma-carousel.min.js"></script>
  <script src="./static/js/bulma-slider.min.js"></script>
  <script src="./static/js/index.js"></script>
</head>

<body>

  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>
    <div class="navbar-menu">
      <div class="navbar-start" style="flex-grow: 1; justify-content: center;">
        <a class="navbar-item" href="https://github.com/infi-coder">
          <span class="icon">
            <i class="fas fa-home"></i>
          </span>
        </a>

        <div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link">
            More
          </a>
          <div class="navbar-dropdown">
            <a class="navbar-item" href="https://github.com/infi-coder">
              InfiCoder Organization
            </a>
          </div>
        </div>
      </div>

    </div>
  </nav>

  <div class="container">
    <div class="column has-text-centered">
      <img style="max-width: 200px; margin-bottom: -50px;" src="static/images/inficoder_eval_logo3.png">
    </div>
  </div>

  <section class="hero">
    <div class="hero-body">
      <div class="container is-max-desktop">
        <div class="columns is-centered">
          <div class="column has-text-centered">
            <h1 class="title is-1 publication-title">InfiBench: Evaluating the Question-Answering Capabilities of Code LLMs
            </h1>
            <div class="is-size-5 publication-authors">
              <span class="author-block">
                The InfiCoder Team
              </span>
              <br>
              <!-- <span class="author-block">
                Main Maintainer: <a href="mailto:xxxxx">xxxxx</a>
              </span> -->
              <!-- <span class="author-block">
                <a href="https://xxx.github.io/">xxxxxx</a><sup>1</sup></span>
			        <br/> -->
            </div>

            <div class="is-size-5 publication-authors">
              <!-- <span class="author-block"><sup>1</sup>Caption of Quận 5, Ho Chi Minh City, Vietnam</span> -->
              <!-- <span class="author-block"><sup>2</sup>Peking University,</span> -->
            </div>

            <div class="column has-text-centered">
              <div class="publication-links">
                <!-- PDF Link. -->
                <span class="link-block">
                  <a href="https://arxiv.org/abs/2404.07940"
                    class="external-link button is-normal is-rounded is-dark" target='_blank'>
                    <span class="icon">
                      <i class="ai ai-arxiv"></i>
                    </span>
                    <span>Report</span>
                  </a>
                </span>
                <!-- Dataset Link. -->
                <span class="link-block">
                  <a href="https://github.com/infi-coder/infibench-evaluation-harness/"
                     class="external-link button is-normal is-rounded is-dark" target='_blank'>
                    <span class="icon">
                      <i class="fab fa-github"></i>
                    </span>
                    <span>Code</span>
                  </a>
                  <!-- <a href="https://github.com/infi-coder/inficoder-eval-framework"
                     class="external-link button is-normal is-rounded is-dark" target='_blank'>
                    <span class="icon">
                      <i class="fab fa-github"></i>
                    </span>
                    <span>Evaluation Repo</span>
                  </a> -->
                </span>
                <!-- Twitter Link. -->
                <!-- <span class="link-block">
                  <a href="https://twitter.com/taoyds/status/1595086401309388801"
                    class="external-link button is-normal is-rounded is-dark">
                    <span class="icon">
                      <i class="fab fa-twitter"></i>
                    </span>
                    <span>Twitter</span>
                  </a>
                </span> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>


  <section class="hero teaser">
    <div class="container is-max-desktop">
      <div class="hero-body">
        <h2 class="subtitle has-text-centered">
          InfiBench is a comprehensive benchmark for code large language models evaluating model ability on answering freeform real-world questions in the code domain.
        </h2>
        <img src="static/images/inficoder-eval-main.png">
      </div>
    </div>
  </section>


  <section class="section">
    <div class="container is-max-desktop">
      <!-- Abstract. -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Overview</h2>
          <div class="content has-text-justified">
            <p>
              Large Language Models for code (code LLMs) have witnessed tremendous progress in recent years. 
              With the rapid development of code LLMs, many popular evaluation benchmarks, such as <a href="https://github.com/openai/human-eval">HumanEval</a>, <a href="https://ds1000-code-gen.github.io/">DS-1000</a>,
              and <a href="https://arxiv.org/abs/2108.07732">MBPP</a>, have emerged to measure the performance of code LLMs with a particular focus on code generation tasks. However, they are insufficient to cover the full range of expected capabilities of code LLMs, which span beyond code generation to answering diverse coding-related questions. To fill this gap, we propose InfiBench, the first large-scale freeform question-answering (QA) benchmark for code to our knowledge, comprising 234 carefully selected high-quality Stack Overflow questions that span across 15 programming languages. InfiBench uses four types of model-free automatic metrics to evaluate response correctness where domain experts carefully concretize the criterion for each question. We conduct a systematic evaluation for over 100 latest code LLMs on InfiBench, leading to a series of novel and insightful findings. Our detailed analyses showcase potential directions for further advancement of code LLMs. InfiBench is fully open source and continuously expanding to foster more scientific and systematic practices for code LLM evaluation.
            </p>
          </div>
        </div>
      </div>
      <!--/ Abstract. -->
    </div>
  </section>


  <section class="section">
    <div class="container is-max-desktop">
      <!-- Example. -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Statistics and Examples</h2>
          <div class="content has-text-justified">
            <p>
              InfiBench comprises 234 carefully picked high-quality Stack Overflow questions, covering 15 programming languages, and largely <b>following the natural question distribution of <a href="https://stackoverflow.com/">Stack Overflow</a></b>.
            </p>

            <img src="static/images/data_domain_stats.png">

            <p>
            <br>
              We recruited five domain experts to create the benchmark and annotate the correctness evaluation criteria.
              Specifically, the InfiBench framework integrates four types of model-free metrics for evaluating the correctness: keywords matching, blank filling, unit testing, and dialogue similarity.
            </p>

            <img src="static/images/data_examples.png">

            <p>
            <br>
              Below is the question type, metric type, and length statistics.
            </p>

            <center>
              <img style="width: 350px" src="static/images/general_statistics.png">
            </center>

          </div>
        </div>
      </div>
      <!--/ Example. -->
    </div>
  </section>

  <section class="section">
    <div class="container is-max-desktop">
      <!-- Comparison. -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Comparison</h2>
          <div class="content has-text-justified">
            <p>Existing benchmarks weigh heavily on code generation, unit-test-based evaluation, and a limited set of programming languages. InfiCoder-Eval processes a much higher diversity to reflect real-world code LLMs’ usage scenarios and is far from saturation.</p>
            <img src="static/images/comparison.png">
          </div>
        </div>
      </div>
      <!--/ Comparison. -->
    </div>
  </section>


  <section class="section">
    <div class="container is-max-desktop">
      <!-- Perturbation and Prompt. -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Prompts and Evaluation Protocol</h2>
          <div class="content has-text-justified">
            Each question contains a system prompt and content prompt.
            For questions whose responses are mainly in natural language, the system prompt is
            <div class="highlighter-rouge">
              <div class="highlight">
                <code>You are a professional assistant for programmers. By default, questions and answers are in Markdown format. You are chatting with programmers, so please answer as briefly as possible.
                </code>
              </div>
            </div>
            For other questions, the system prompt is
            <div class="highlighter-rouge">
              <div class="highlight">
                <code>You are a professional assistant for programmers. By default, questions and answers are in Markdown format.
                </code>
              </div>
            </div>
            We then format the system prompt and content prompt following each model's default instruction template.
            If no instruction template specified, we use the prompt format 
            <div class="highlight">
              <code>{system prompt}\n{content prompt}
              </code>
            </div>
            <p>We adopt <b>best@10</b> as the main evaluation metric, where 10 responses are sampled and evaluated for each question and the best score per question is recorded and summed up.
              Throughout the evaluation, we set <b>sampling temperature T to be 0.2 and top p cut-off threshold to be 0.9</b>.
              We leave the exploration of other hyperparameters as the future work.
            </p>
            <p>For score computation, we treat each question equally with one point each.
              <b>Since the question frequency largely follows the Stack Overflow distribution, this score can be explained as how well the model responds to Stack Overflow questions.</b>
              Given 234 questions in the benchmark, the full score is 234, and we by default report the percentage score (achieved score divided by the full score which is 234).
              The one point for each question can be further decomposed into a few scoring points within each question.
              For example, a question may contain four keywords with weights 2, 1, 1, and 1 each.
              Then, matching each keyword can contribute to 0.4, 0.2, 0.2, and 0.2 points respectively to the final score.
            </p>
          </div>
        </div>
      </div>
      <!--/ Perturbation and Prompt. -->
    </div>
  </section>

  <section class="section">
    <div class="container is-max-desktop">
        <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Leaderboard</h2>
        </div>
      </div>
    </div>
    <br>
    <div class="container is-max-desktop has-text-justified">
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <div>
            <img src="static/images/all_results.png">
          </div>
          <p>Each point corresponds to an open-source model, with error bars for those smaller than 30B. Each dotted segment corresponds to an MoE model. Proprietary models shown as lines with uncertainty ranges.</p>
        </div>
      </div>
    </div>
    <div class="cover" id="contentCover">
      <!-- Baseline. -->
      <div class="container-t">
        <div class="row">
          <div class="col-md-12">
            <div class="infoCard">
              <div class="infoBody">
                <p align="left">
                  <div class="left"><b>Notice</b>: we set the max tokens to generate=1024 (since GPT4 generates 662 tokens without the constraint, we provide some wiggle room by setting to 1024 tokens)
                  </div>
                </p>
                <p align="left">
                  <div class="left">For models with >30B parameters, we evaluate once due to resource limit, otherwise we evaluate three times and report the mean and standard deviation.
                  </div>
                </p>
                <p align="left">
                  <div class="left"><i class="fa fa-lock"></i> stands for proprietary models.</div>
                </p>
                <br>
                <table class="table maintable stripe hover row-border order-column" id="maintable">
                  <thead>
                    <tr>
                      <th>Rank</th>
                      <th>Model Name</th>
                      <th># Params. (in B)</th>
                      <th>Context Length</th>
                      <th>Full Set Score</th>
                      <th>Full Set Std</th>
                      <th></th>
                    </tr>
                  </thead>
                  <tbody>
                    {% for item in site.data.leaderboard.records %}
                    <tr>
                      <td>{{ item.rank }}</td>
                      {% if item.link != null %}
                        <td>{% if item.locked %}<i class="fa fa-lock"></i>{% endif %}<a href="{{ item.link }}">{{ item.title }}</a></td>
                      {% else %}
                        <td>{% if item.locked %}<i class="fa fa-lock"></i>{% endif %}{{ item.title }}</td>
                      {% endif %}
                      {% if item.size != null %}
                        <td>{{ item.size }}</td>
                      {% else %}
                        <td>/</td>
                      {% endif %}
                      <td>{{ item.ctx_length }}</td>
                      <td>{{ item.score }}</td>
                      {% if item.score_std != null %}
                        <td>{{ item.score_std }}</td>
                      {% else %}
                        <td></td>
                      {% endif %}
                      <td>{{ item.comment }}</td>
                    </tr>
                    {% endfor %}
                  </tbody>
                </table>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container is-max-desktop">
      <!-- Benchmarking Tutorial -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Try the Benchmark!</h2>
          <p>Note: we only support Linux environment yet.</p>
          <div class="content has-text-justified">
            <ol>
              <li>Convert or save your model weights in Hugging Face Transformers format.</li>
              <li>Clone our <a href="https://github.com/infi-coder/infibench-evaluation-harness">code repository</a>.</li>
              <li>Follow the <a href="https://github.com/infi-coder/infibench-evaluation-harness?tab=readme-ov-file#features-and-tutorials">short tutorial</a> to generate responses and evaluate on InfiBench!</li>
            </ol>
          </div>
        </div>
      </div>
      <!--/ Benchmarking Tutorial -->
    </div>
  </section>

  <!-- <section class="section" id="Acknowledgement">
    <div class="container is-max-desktop content">
      <div class="bibtex-body">
        <h2 class="title">Acknowledgement</h2>
        <p>...</p>
      </div>
    </div>
  </section> -->


  <section class="section">
    <div class="container is-max-desktop">
      <!-- Benchmarking Tutorial -->
      <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
          <h2 class="title is-3">Feedback</h2>
          <div class="content has-text-justified">
            <script src="https://giscus.app/client.js"
                    data-repo="infi-coder/inficoder-eval"
                    data-repo-id="R_kgDOKxa6cg"
                    data-category-id="DIC_kwDOKxa6cs4CbSFx"
                    data-mapping="pathname"
                    data-strict="0"
                    data-reactions-enabled="1"
                    data-emit-metadata="0"
                    data-input-position="bottom"
                    data-theme="preferred_color_scheme"
                    data-lang="en"
                    crossorigin="anonymous"
                    async>
            </script>
            <br>
            <p>You can also give us feedback in the discussion issue posts of our repositories:</p>
            <ul>
              <li><a href="https://github.com/infi-coder/inficoder-eval/issues/1"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Finfi-coder%2Finficoder-eval%2Fissues%2F1?label=General%20Discussion"></a></li>
              <!-- <li><a href="https://github.com/infi-coder/ffqa-evaluation-harness/issues/1"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Finfi-coder%2Finficoder-eval?label=Inference%20Framework%20Discussion"></a></li>
              <li><a href="https://github.com/infi-coder/inficoder-eval-framework/issues/1"><img alt="Static Badge" src="https://img.shields.io/badge/https%3A%2F%2Fgithub.com%2Finfi-coder%2Finficoder-eval?label=Evaluation%20Framework%20Discussion"></a></li> -->
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="section" id="BibTeX">
    <div class="container is-max-desktop content">
      <div class="bibtex-body">
        <h2 class="title">BibTeX</h2>
        <pre><code>@misc{inficodereval,
  author = {InfiCoderTeam},
  title = {InfiBench: Evaluating the Question-Answering Capabilities of Code LLMs},
  year = {2024},
  publisher = {Github Pages},
  howpublished = "\url{https://infi-coder.github.io/infibench/}"
}</code></pre>
      </div>
    </div>
  </section>


  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <a class="icon-link" href="https://arxiv.org/abs/2404.07940">
          <i class="fas fa-file-pdf" style="color:white"></i>
        </a>
        <a class="icon-link" href="https://github.com/infi-coder" class="external-link" disabled>
          <i class="fab fa-github" style="color:white"></i>
        </a>
      </div>
      <div class="columns is-centered">
        <div class="column is-8">
          <div class="content">
            <p>
              This website is adapted from <a href="https://ds1000-code-gen.github.io/">ds1000-code-gen.github.io</a> and is licensed under a <a rel="license"
                href="http://creativecommons.org/licenses/by-sa/4.0/">Creative
                Commons Attribution-ShareAlike 4.0 International License</a>.
            </p>
            <p>
              This means you are free to borrow the <a href="https://github.com/infi-coder/infibench">source
                code</a> of this website,
              we just ask that you link back to this page in the footer.
            </p>
          </div>
        </div>
      </div>
    </div>
  </footer>
  
  <script>
    $(document).ready( function () {
      $('.mainTable').DataTable({ordering: true, order: [[4, 'desc']], columns: [{ "type": "num" },{ "type": "html" },{ "type": "num" },{ "type": "num-fmt" },{ "type": "num-fmt" },{ "type": "num-fmt" },{ "type": "html", "orderable": false }]});
    } );
  </script>

</body>

</html>
