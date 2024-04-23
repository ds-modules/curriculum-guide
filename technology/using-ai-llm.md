# Utilizing Large Language Models (LLMs) in Datahub

Currently, the Datahub infrastructure team does not support the deployment of Large Language Models (LLMs) in courses utilizing Datahub. The limited compute resources available to courses, coupled with the unavailability of TPUs/GPUs, make it challenging to deploy language models in Datahub. Additionally, this could lead to a disproportionate increase in cloud costs, complicating operations.

As part of their course assignments, Data 100 deployed a smaller language model known as DistilBERT. Here is an [example notebook](https://data100.datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDS-100%2Fsp24-student&urlpath=lab%2Ftree%2Fsp24-student%2F%2Fhw%2Fhw03%2Fhw03.ipynb&branch=main) using distiBERT.  To ensure that course operations were not affected, CPU resources had to be bumped. If you're considering the use of language models or any AI model as part of your teaching workflow, we strongly recommend scheduling a consultation with the Datahub team at the start of the semester or a few weeks prior to the assignment release. This proactive approach will greatly assist us in determining whether we can provide support, and if so, what optimizations need to be implemented on our end to ensure a smooth experience for both you and your students.


