<div align="center">
<h2>
Synthetic Singers
    
A Review of Deep-Learning-based Singing Voice Synthesis Approaches
</h2>
</div>

This repository contains the resources for paper **Synthetic Singers: A Review of Deep-Learning-based Singing Voice Synthesis Approaches**.

For more details, please refer to the [paper]().

## 🚀 Quick Start

- [Tasks of SVS](#tasks-of-svs)
- [Architectures of SVS Systems](#architectures-of-svs-systems)
- [SVS Representations and Control](#svs-representations-and-control)
- [Resources in SVS Models](#resources-in-svs-models)
  - [Open-Source Datasets](#open-source-datasets)
  - [Annotation Tools for Singing Data](#annotation-tools-for-singing-data)

And the organiztion of this survey is shown below. 

<div align='center'>
<img src="figure/organization.png" alt="img1-organization" style="zoom: 20%;" />

Figure 1: Organization of the survey.
</div>

## Tasks of SVS

The mainstream singing voice tasks can be broadly categorized into the following four types:

* **Hi-Fidelity Synthesis:** Focuses on generating high-quality singing voices, with emphasis on clear articulation, natural prosody, and accurate pitch rendering.
* **Controllable Synthesis:** Aims to maintain synthesis quality while enabling fine-grained control over attributes such as timbre, style, and vocal techniques.
* **Singing Style Transfer:** Given a reference singing prompt, the goal is to generate a synthetic voice that closely matches the reference in terms of timbre, style, and expression.
* **Text-to-Song Generation:** Targets the joint generation of high-quality singing voices and their aligned accompaniment, producing a complete musical piece from text input.


<div align='center'>
<img src="figure/tasks.png" alt="img2-tasks" style="zoom: 20%;" />

Figure 2: An overall demonstration of four prevailing tasks of SYS sytem.
</div>

## Architectures of SVS Systems

We categorize current SVS systems into two types based on whether a vocoder is explicitly used in the synthesis pipeline: (a) **Cascaded SVS Models** and (b) **End-to-End SVS Models**.

<div align='center'>
<img src="figure/arch.png" alt="img3-architecture" style="zoom: 20%;" />

Figure 3: We categorize SVS models into two paradigms, cascaded and end-to-end approaches, based on whether the
model can directly generate the waveform without the use of vocoder. Dashed lines represent optional processes.
</div>

## Publicly Available Singing Voice Synthesis Models

<div align='center'>
<table>
    <thead>
        <tr>
            <th>Model</th>
            <th>URL</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>DiffSinger</td>
            <td><a href="https://github.com/MoonInTheRiver/DiffSinger">https://github.com/MoonInTheRiver/DiffSinger</a></td>
        </tr>
        <tr>
            <td>VISinger (Unofficial implementation)</td>
            <td><a href="https://github.com/So-Fann/VISinger">https://github.com/So-Fann/VISinger</a></td>
        </tr>
        <tr>
            <td>VISinger 2</td>
            <td><a href="https://github.com/zhangyongmao/VISinger2">https://github.com/zhangyongmao/VISinger2</a></td>
        </tr>
        <tr>
            <td>VI-SVS</td>
            <td><a href="https://github.com/PlayVoice/VI-SVS">https://github.com/PlayVoice/VI-SVS</a></td>
        </tr>
        <tr>
            <td>NNSVS</td>
            <td><a href="https://github.com/nnsvs/nnsvs">https://github.com/nnsvs/nnsvs</a></td>
        </tr>
        <tr>
            <td>StyleSinger</td>
            <td><a href="https://github.com/AaronZ345/StyleSinger">https://github.com/AaronZ345/StyleSinger</a></td>
        </tr>
        https://github.com/NZqian/RapBank
        <tr>
            <td>TCSinger</td>
            <td><a href="https://github.com/AaronZ345/TCSinger">https://github.com/AaronZ345/TCSinger</a></td>
        </tr>
        <tr>
            <td>TCSinger 2</td>
            <td><a href="https://github.com/AaronZ345/TCSinger2">https://github.com/AaronZ345/TCSinger2</a></td>
        </tr>
        <tr>
            <td>FreeStyler</td>
            <td><a href="https://github.com/NZqian/RapBank">https://github.com/NZqian/RapBank</a></td>
        </tr>
        <tr>
            <td>AlignSTS</td>
            <td><a href="https://github.com/RickyL-2000/AlignSTS">https://github.com/RickyL-2000/AlignSTS</a></td>
        </tr>
        <tr>
            <td>ComoSpeech</td>
            <td><a href="https://github.com/zhenye234/CoMoSpeech">https://github.com/zhenye234/CoMoSpeech</a></td>
        </tr>
       <tr>
            <td>ExpressiveSinger</td>
            <td><a href="https://github.com/ExpressiveSinger/ExpressiveSinger">https://github.com/ExpressiveSinger/ExpressiveSinger</a></td>
        </tr>
        <tr>
            <td>TechSinger</td>
            <td><a href="https://github.com/gwx314/TechSinger">https://github.com/gwx314/TechSinger</a></td>
        </tr>
        <tr>
            <td>Prompt-Singer</td>
            <td><a href="https://github.com/cyanbx/Prompt-Singer">https://github.com/cyanbx/Prompt-Singer</a></td>
        </tr>
        <tr>
            <td>HiFiSinger</td>
            <td><a href="https://github.com/microsoft/muzic">https://github.com/microsoft/muzic</a></td>
        </tr>
        <tr>
            <td>HiFiSinger (Unofficial implementation)</td>
            <td><a href="https://github.com/CODEJIN/HiFiSinger">https://github.com/CODEJIN/HiFiSinger</a></td>
        </tr>
        <tr>
            <td>ByteSing</td>
            <td><a href="https://github.com/Noise-Labs/ByteSing-pytorch">https://github.com/Noise-Labs/ByteSing-pytorch</a></td>
        </tr>
        <tr>
            <td>WeSinger</td>
            <td><a href="https://zzw922cn.github.io/wesinger/">https://zzw922cn.github.io/wesinger/</a></td>
        </tr>
        <tr>
            <td>SingGAN</td>
            <td><a href="https://github.com/Rongjiehuang/SingGAN">https://github.com/Rongjiehuang/SingGAN</a></td>
        </tr>
        <tr>
            <td>UniSinger</td>
            <td><a href="https://github.com/ViEm-ccy/UniSinger">https://github.com/ViEm-ccy/UniSinger</a></td>
        </tr>
        <tr>
            <td>Learn2Sing 2.0</td>
            <td><a href="https://github.com/WelkinYang/Learn2Sing2.0">https://github.com/WelkinYang/Learn2Sing2.0</a></td>
        </tr>
        <tr>
            <td>UniSyn</td>
            <td><a href="https://github.com/codejiajia/UniSyn">https://github.com/codejiajia/UniSyn</a></td>
        </tr>
        <tr>
            <td>NaturalSpeech 2</td>
            <td><a href="https://github.com/lucidrains/naturalspeech2-pytorch">https://github.com/lucidrains/naturalspeech2-pytorch</a></td>
        </tr>
        <tr>
            <td>YuE</td>
            <td><a href="https://github.com/multimodal-art-projection/YuE">https://github.com/multimodal-art-projection/YuE</a></td>
        </tr>
        <tr>
            <td>SpeechGPT-Gen</td>
            <td><a href="https://github.com/0nutation/SpeechGPT">https://github.com/0nutation/SpeechGPT</a></td>
        </tr>
       <tr>
            <td>InsprieMusic</td>
            <td><a href="https://github.com/FunAudioLLM/InspireMusic">https://github.com/FunAudioLLM/InspireMusic</a></td>
        </tr>
        <tr>
            <td>Songgen</td>
            <td><a href="https://github.com/LiuZH-19/SongGen">https://github.com/LiuZH-19/SongGen</a></td>
        </tr>
        <tr>
            <td>DiffRhythm</td>
            <td><a href="https://github.com/ASLP-lab/DiffRhythm">https://github.com/ASLP-lab/DiffRhythm</a></td>
        </tr>
        <tr>
            <td>Levo</td>
            <td><a href="https://huggingface.co/tencent/SongGeneration">https://huggingface.co/tencent/SongGeneration</a></td>
        </tr>
    </tbody>
</table>

Table 1: The list of publicly available SVS models and their URL
</div>

## SVS Representations and Control

## Resources in SVS Models

In this section, we provide an overview of currently available open-source datasets, as well as publicly accessible singing voice annotation and preprocessing tools.

### Open-Source Datasets

| name | paper | year | url |
|--------------------|---------------------------------------------------------------------------------------------------------------------------|------|------------------------------------------------------------------------------|
| MIR-1K             | On the Improvement of Singing Voice Separation for Monaural Recordings Using the MIR-1K Dataset                           | 2009 |                                                                              |
| NUS-48E            | The NUS Sung and Spoken Lyrics Corpus:A Quantitative Comparison of Singing and Speech                                     | 2013 |                                                                              |
| VocalSet           | VocalSet: A Singing Voice Dataset                                                                                         | 2018 | https://zenodo.org/records/1203819                                           |
| KVT                | Semantic Tagging of Singing Voices in Popular Music Recordings                                                            | 2020 |                                                                              |
| CSD                | Children's Song Dataset for Singing Voice Research                                                                        | 2020 | https://zenodo.org/record/4785016#.YLYW6P0QtTa                               |
| PJS                | PJS: phoneme-balanced Japanese singing voice corpus                                                                       | 2020 | https://sites.google.com/site/shinnosuketakamichi/research-topics/pjs_corpus |
| NHSS               | NHSS: A Speech and Singing Parallel Database                                                                              | 2021 | https://hltnus.github.io/NHSSDatabase/download.html                          |
| OpenSinger         | Multi-Singer: Fast Multi-Singer Singing Voice Vocoder With A Large-Scale Corpus                                           | 2021 | https://multi-singer.github.io/                                              |
| Tohoku Kiritan     | Tohoku Kiritan singing database: A singing database for statistical parametric singing synthesis using Japanese pop songs | 2021 | https://zunko.jp/kiridev/login.php                                           |
| PopCS              | DiffSinger: Singing Voice Synthesis via Shallow Diffusion Mechanism                                                       | 2022 |                                                                              |
| M4Singer           | M4Singer: a Multi-Style, Multi-Singer and Musical Score Provided Mandarin Singing Corpus                                  | 2022 | https://github.com/M4Singer/M4Singer                                         |
| PopBuTFy           | Learning the Beauty in Songs: Neural Singing Voice Beautifier                                                             | 2022 | https://github.com/MoonInTheRiver/NeuralSVB                                  |
| Opencpop           | Opencpop: A High-Quality Open Source Chinese Popular Song Corpus for Singing Voice Synthesis                              | 2022 | https://wenet.org.cn/opencpop/                                               |
| Annotated-VocalSet | Annotated-VocalSet: A Singing Voice Dataset                                                                               | 2022 | https://zenodo.org/records/7061507                                           |
| SingStyle111       | SINGSTYLE111: A MULTILINGUAL SINGING DATASET WITH STYLE TRANSFER                                                          | 2023 |                                                                              |
| GTSinger           | GTSinger: A Global Multi-Technique Singing Corpus with Realistic Music Scores for All Singing Tasks                       | 2024 | https://huggingface.co/datasets/GTSinger/GTSinger                            |
| AceSinger          | Singing Voice Data Scaling-up: An Introduction to ACE-Opencpop and ACE-KiSing                                             | 2024 | https://github.com/espnet/espnet                                             |

### Annotation Tools for Singing Data

| Name     | Usage                          | Link |
|----------|--------------------------------|------|
| MFA      | Speech-Text Forced Alignment   | https://montrealcorpustools.github.io/Montreal-Forced-Aligner/    |
| SOFA     | Singing-Text Forced Alignment  |  https://github.com/qiuqiao/SOFA  |
| VOCANO   | Vocal's Note Transcription     | https://github.com/B05901022/VOCANO  |
| MusicYOLO| Music's Note Transcription     |  https://github.com/itec-hust/MusicYOLO  |
| ROSVOT   | Vocal's Note Transcription     | https://github.com/RickyL-2000/ROSVOT   |
| STARS    | Unified Model for Annotation   | https://github.com/gwx314/STARS  |
| UVR |  Voice and Accompaniment Separation | https://ultimatevocalremover.com/ |
| ClearerVoice | Voice Enhancement | https://github.com/modelscope/ClearerVoice-Studios |
