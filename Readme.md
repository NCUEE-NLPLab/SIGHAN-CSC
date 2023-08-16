# Chinese Spell Checking
## Introduction
Chinese spelling errors frequently arise from confusion among multiple-character words that are phonologically and visually similar but semantically distinct. The first Chinese Spelling Check (CSC) bakeoff was organized as part the Seventh SIGHAN (Special Interesting Group on Chinse Language Processing of the Association for Computational Linguistics) workshop (Wu et al., 2013). This shared task is the first open evaluation for automatic Chinese spelling checkers. A second version of this bakeoff was collocated with the Third CIPS-SIGHAN Joint Conference on Chinese Language Processing (Yu et al., 2014). A third one was organized in conjunction with the Eighth SIGHAN workshop (Tseng et al. 2015). The main purpose of these bakeoffs was to provide a common setting so that researchers who approach the tasks with different linguistic factors and computational techniques can compare their results. <br>
Different from the initial edition in SIGHAN 2013 adopting the data sets written by Chinese native speakers, the second and third bakeoffs used the TOCFL Learner Corpus as the data source. This is considered a greater challenge in detecting and correcting spelling errors as the sentences written by Chinese as a foreign language learners can contain errors that are hard to predict. The goal is identical to evaluate the capability of a Chinese spelling checker. A sentence consisting of several clauses with/without spelling errors was given as the input. The checker should return the locations of incorrect characters and suggest the correct characters. Each character or punctuation mark occupies 1 spot for counting location.

## Summary

<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow">Shared Task</th>
    <th class="tg-c3ow">SIGHAN 2013<br>(Wu et al., 2013)</th>
    <th class="tg-c3ow">SIGHAN 2014<br>(Yu et al., 2014)</th>
    <th class="tg-c3ow">SIGHAN 2015<br>(Tseng et al., 2015)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">Examples</td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">Input: (NID=88888) 擁有六百一十年歷史 的崇禮門，象微著南韓人的精神，在一 夕之門，被火燒得精光。</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">Output: 88888, 16, 徵 29, 間</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">Input: (pid=B1-0201-1) 我一身中的貴人就是我姨媽，從我回來台灣的時候， 她一只都很照顧我，也很觀心我。</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">Output: B1-0201-1, 3, 生, 26, 直, 35, 關</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">Input: (pid=B2-1670-2) 在日本，大學生打工的情況 是相當普偏的。</span> <br><span style="font-weight:400;font-style:normal;text-decoration:none">Output: B2-1670-2, 17, 遍</span></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Data Source</td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">Chinese native speakers’ data</span></td>
    <td class="tg-c3ow" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none">TOCFL Learner Corpus</span></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Training Set</td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">This set included 700 samples selected from students’ essays. Besides, the set of Chinese characters with similar shapes/pronunciations was provided.</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">This set included 1,301 sentences with a total of 5,284 spelling errors</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">This set included 970 sentences with a total of 3,143 spelling errors</span></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Test Set</td>
    <td class="tg-c3ow">This set consisted of 2,000 testing sentences for both subtasks, each with an average of 70 characters. Total number of error character is 1,641.</td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none">This set consisted of 1,062 testing sentences, each with an average of 50 characters. One half contained no spelling errors, while the other half included as least one spelling error each for a total of 792 spelling errors.</span></td>
    <td class="tg-c3ow">This set consisted of 1,100 testing sentences. Half of these sentences contained no spelling errors, while the other half included as least one spelling errors.</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Evaluation Metrics</td>
    <td class="tg-c3ow" colspan="3">False Positive Rate, Detection-level Accuracy/Precision/Recall/F1,<br>Correction-level Accuracy/Precision/Recall/F1.</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Registered Teams</td>
    <td class="tg-c3ow">17 teams (9 from Taiwan, 5 from China and 3 from Singapore, Japan, and UK)</td>
    <td class="tg-c3ow">19 teams (10 from China, 8 from Taiwan, and 1 private firm)</td>
    <td class="tg-c3ow">9 teams (4 from China, 4 from Taiwan, and 1 private firm)</td>
  </tr>
</tbody>
</table>

## Citations
* [SIGHAN 2013] Shih-Hung Wu, Chao-Lin Liu, and Lung-Hao Lee (2013). [Chinese Spelling Check Evaluation at SIGHAN Bake-off 2013](https://aclanthology.org/W13-4406.pdf). In *Proceedings of SIGHAN'13*, pp. 35-42. 
* [SIGHAN 2014] Liang-Chih Yu, Lung-Hao Lee, Yuen-Hsien Tseng and Hsin-Hsi Chen (2014). [Overview of SIGHAN 2014 Bake-off for Chinese Spelling Check](https://aclanthology.org/W14-6820.pdf) . In *Proceedings of CLP'14*, pp. 126-132.
* [SIGHAN 2015] Yuen-Hsien Tseng, Lung-Hao Lee, Li-Ping Chang, and Hsin-Hsi Chen (2015). [Introduction to SIGHAN 2015 Bake-off for Chinese Spelling Check](https://aclanthology.org/W15-3106.pdf). In *Proceedings of SIGHAN'15*, pp. 32-37.
* [ICCE 2019] Lung-Hao Lee, Wun-Syuan Wu, Jian-Hong Li, Yu-Chi Lin, and Yuen-Hsien Tseng (2019). [Building a Confused Character Set for Chinese Spell Checking.](https://www.researchgate.net/publication/339068842_Building_a_Confused_Character_Set_for_Chinese_Spell_Checking_) In *Proceedings of ICCE'19*, pp. 703-705.


