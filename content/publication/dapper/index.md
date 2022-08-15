---
title: 'DAPPER: Performance Estimation of Domain Adaptation in Mobile Sensing'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Taesik Gong
  - admin
  - Adiba Orzikulova
  - Yunxin Liu
  - Sung Ju Hwang
  - Jinwoo Shin
  - SungJu Lee

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2021-11-22T08:49:33Z'
# doi: 'https://doi.org/10.48550/arXiv.2111.11053'

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 
# 0 = Uncategorized
# 1 = Preprint / Working Paper
# 2 = Conferences and Journals
# 3 = Posters, Demos, Videos, and Workshop Papers 
# 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: ArXiv
publication_short: ArXiv

abstract: Many applications that utilize sensors in mobile devices and apply machine learning to provide novel services have emerged. However, various factors such as different users, devices, environments, and hyperparameters, affect the performance for such applications, thus making the domain shift (i.e., distribution shift of a target user from the training source dataset) an important problem. Although recent domain adaptation techniques attempt to solve this problem, the complex interplay between the diverse factors often limits their effectiveness. We argue that accurately estimating the performance in untrained domains could significantly reduce performance uncertainty. We present DAPPER (Domain AdaPtation Performance EstimatoR) that estimates the adaptation performance in a target domain with only unlabeled target data. Our intuition is that the outputs of a model on the target data provide clues for the model's actual performance in the target domain. DAPPER does not require expensive labeling costs nor involve additional training after deployment. Our evaluation with four real-world sensing datasets compared against four baselines shows that DAPPER outperforms the baselines by on average 17% in estimation accuracy. Moreover, our on-device experiment shows that DAPPER achieves up to 216X less computation overhead compared with the baselines.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Website
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2111.11053.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
