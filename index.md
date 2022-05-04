## Publications


### FaST: A linear time stack trace alignment heuristic for crash report deduplication
*Irving Muller Rodrigues, Daniel Aloise, and Eraldo Rezende Fernandes*

[PDF](https://irving-muller.github.io/papers/FaST.pdf) ‖ [Github](https://github.com/irving-muller/FaST) 

In software projects, applications are often monitored by systems that automatically identify crashes, collect their information into reports, and submit them to developers. Especially in popular applications, such systems tend to generate a large number of crash reports in which a significant portion of them are duplicate. Due to this high submission volume, in practice, the crash report deduplication is supported by devising automatic systems whose efficiency is a critical constraint. In this paper, we focus on improving deduplication system throughput by speeding up the stack trace comparison. In contrast to the state-of-the-art techniques, we propose FaST , a novel sequence alignment method that computes the similarity score between two stack traces in linear time. Our method independently aligns identical frames in two stack traces by means of a simple alignment heuristic. We evaluate FaST and five competing methods on four datasets from open-source projects using ranking and binary metrics. Despite its simplicity, FaST consistently achieves state-of-the-art performance regarding all metrics considered. Moreover, our experiments confirm that FaST is substantially more efficient than methods based on optimal sequence alignment.




### Tracesim: An alignment method for computing stack trace similarity
*Irving Muller Rodrigues, Aleksandr Khvorov, Daniel Aloise, Roman Vasiliev, Dmitrij Koznov, Eraldo Rezende Fernandes, George Chernishev, Dmitry Luciv, and Nikita Povarov*

[PDF](https://link.springer.com/article/10.1007/s10664-021-10070-w) ‖ [Github](https://github.com/irving-muller/TraceSim_EMSE) 

Software systems can automatically submit crash reports to a repository for investigation when program failures occur. A significant portion of these crash reports are duplicate, i.e., they are caused by the same software issue. Therefore, if the volume of submitted reports is very large, automatic grouping of duplicate crash reports can significantly ease and speed up analysis of software failures. This task is known as crash report deduplication. Given a huge volume of incoming reports, increasing quality of deduplication is an important task. The majority of studies address it via information retrieval or sequence matching methods based on the similarity of stack traces from two crash reports. While information retrieval methods disregard the position of a frame in a stack trace, the existing works based on sequence matching algorithms do not fully consider subroutine global frequency and unmatched frames. Besides, due to data distribution differences among software projects, parameters that are learned using machine learning algorithms are necessary to provide more flexibility to the methods.

In this paper, we propose TraceSim – an approach for crash report deduplication which combines TF-IDF, optimum global alignment, and machine learning (ML) in a novel way. Moreover, we propose a new evaluation methodology for this task that is more comprehensive and robust than previously used evaluation approaches. TraceSim significantly outperforms seven baselines and state-of-the-art methods in the majority of the scenarios. It is the only approach that achieves competitive results on all datasets regarding all considered metrics. Moreover, we conduct an extensive ablation study that demonstrates the importance of each TraceSim’s element to its final performance and robustness. Finally, we provide the source code for all considered methods and evaluation methodology as well as the created datasets.



### A Soft Alignment Model for Bug Deduplication
*Irving Muller Rodrigues, Daniel Aloise, Eraldo Rezende Fernandes, and Michel Dagenais*

[PDF](https://irving-muller.github.io/papers/MSR2020.pdf) ‖ [Github](https://github.com/irving-muller/soft_alignment_model_bug_deduplication) 

Bug tracking systems (BTS) are widely used in software projects. An important task in such systems consists in identifying duplicate bug reports, i.e., distinct reports related to the same software issue. For several reasons, reporting bugs that have already been reported is quite frequent, making their manual triage unpractical in large BTSs. In this paper, we present a novel deep learning network based on soft-attention alignment to improve duplicate bug report detec- tion. Our model can dynamically focus on distinct segments of the bug reports during the generation of report representations. This architecture is more flexible than previous approaches that compute report representations without or with limited data exchange. We evaluate our model on four well-known datasets derived from BTSs of four popular open-source projects. Our experimental evaluation relies on a ranking-based methodology, which is more adherent to real world scenarios than decision-making methodologies used in many previous works. It demonstrates that our model outperforms state-of-the-art systems and strong baselines in different scenarios. Finally, we also report on ablation studies to confirm our hypothesis that a more flexible architecture is helpful for extracting relevant information from bug reports.

---
<!-- <p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p> -->
<!-- Remove above link if you don't want to attibute -->
