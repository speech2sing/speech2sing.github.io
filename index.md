# Self-Supervised Singing Voice Pre-Training towards Speech-to-Singing Conversion

<!-- Google tag (gtag.js) -->
<!-- <script async src="https://www.googletagmanager.com/gtag/js?id=G-86MF0006K1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-86MF0006K1');
</script> -->

## Abstract

Speech-to-singing voice conversion (STS) task always suffers from data scarcity, because it requires paired speech and singing data. Compounding this issue are the challenges of content-pitch alignment and the suboptimal quality of generated outputs, presenting significant hurdles in STS research. This paper presents **SVPT**, an STS approach boosted by a self-supervised singing voice pre-training model.
We leverage spoken language model techniques to tackle the rhythm alignment problem and the in-context learning capability to achieve zero-shot conversion. We adopt discrete-unit random resampling and pitch corruption strategies, enabling training with unpaired singing data and thus mitigating the issue of data scarcity. SVPT also serves as an effective backbone for singing voice synthesis (SVS), offering insights into scaling up SVS models. Experimental results indicate that SVPT delivers notable improvements in both STS and SVS endeavors. 


## Speech-to-Singing Conversion with English Samples

* We're beautiful like diamonds in the sky

    <table style='width: 66%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/3.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>(Wu and Yang, 2020)</th>
            <th>AlignSTS</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/wu/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/alignsts/3.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/svpt/3.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

* Oh pretty baby don't bring me down I pray

    <table style='width: 66%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/1.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>(Wu and Yang, 2020)</th>
            <th>AlignSTS</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/wu/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/alignsts/1.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/svpt/1.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

* You don't have to change a single thing

    <table style='width: 66%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/2.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>(Wu and Yang, 2020)</th>
            <th>AlignSTS</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/wu/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/alignsts/2.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/svpt/2.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

## Speech-to-Singing Conversion with Mandarin Samples

* 你 不 知 道 我 为 什 么 狠 下 心

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/4.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/4.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/zh/4.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

* 欣 赏 你 流 浪 像 是 种 信 仰

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/5.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/5.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/zh/5.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

* 不 要 人 山 人 海 热 情 的 尖 叫

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/6.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/6.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/zh/6.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

* 不 问 缘 由 不 管 当 时

    <table style='width: 100%;'>
        <thead>
        <tr>
            <th></th>
            <th>GT</th>
            <th>Speech</th>
            <th>SVPT</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <th scope="row">wav</th>
            <td><audio controls="" ><source src="resources/audio/gt/7.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/speech/7.wav" type="audio/wav"></audio></td>
            <td><audio controls="" ><source src="resources/audio/zh/7.wav" type="audio/wav"></audio></td>
        </tr>
        </tbody>
    </table>

