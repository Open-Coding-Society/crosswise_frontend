---
layout: tailwind
search_exclude: true
hide: true
show_reading_time: false
permalink: /apidocumentation
---

<div class="space-y-8">
  <section class="bg-dark rounded-lg p-8 shadow-lg">
    <h1 class="text-4xl font-bold text-accent mb-4">CrossWise API Documentation</h1>
    <h2 class="text-2xl text-gray-300 mb-6">Technical Implementation Overview</h2>
    
    <p class="text-gray-200 mb-6">
      This documentation outlines the major technical accomplishments and API components that power the CrossWise Smart Guide application. Our system combines real-time data scraping, machine learning forecasting, and social media monitoring to provide accurate border crossing predictions.
    </p>
  </section>

  <body><div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;dark-mode&quot;:&quot;auto&quot;,&quot;toolbar&quot;:&quot;zoom layers tags lightbox&quot;,&quot;edit&quot;:&quot;_blank&quot;,&quot;xml&quot;:&quot;&lt;mxfile host=\&quot;app.diagrams.net\&quot; agent=\&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/136.0.0.0 Safari/537.36\&quot; version=\&quot;27.1.3\&quot;&gt;\n  &lt;diagram name=\&quot;Page-1\&quot; id=\&quot;5CQVelZoNOVqnUf95dn4\&quot;&gt;\n    &lt;mxGraphModel dx=\&quot;1113\&quot; dy=\&quot;625\&quot; grid=\&quot;1\&quot; gridSize=\&quot;10\&quot; guides=\&quot;1\&quot; tooltips=\&quot;1\&quot; connect=\&quot;1\&quot; arrows=\&quot;1\&quot; fold=\&quot;1\&quot; page=\&quot;1\&quot; pageScale=\&quot;1\&quot; pageWidth=\&quot;850\&quot; pageHeight=\&quot;1100\&quot; math=\&quot;0\&quot; shadow=\&quot;0\&quot;&gt;\n      &lt;root&gt;\n        &lt;mxCell id=\&quot;0\&quot; /&gt;\n        &lt;mxCell id=\&quot;1\&quot; parent=\&quot;0\&quot; /&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-7\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;427.5\&quot; y=\&quot;260\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-8\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;530\&quot; y=\&quot;325\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-10\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;427.5\&quot; y=\&quot;400\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-11\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;310\&quot; y=\&quot;325\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-1\&quot; value=\&quot;Dashboard\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;380\&quot; y=\&quot;310\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-62\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-4\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;427.5\&quot; y=\&quot;190\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-4\&quot; value=\&quot;Border API\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;380\&quot; y=\&quot;220\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-14\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-5\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;586.5\&quot; y=\&quot;260\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-5\&quot; value=\&quot;Weather API\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;539\&quot; y=\&quot;310\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-22\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-12\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;527\&quot; y=\&quot;415\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-31\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-12\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;340\&quot; y=\&quot;415\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-12\&quot; value=\&quot;Live Feed API\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;380\&quot; y=\&quot;400\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-45\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-13\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;170\&quot; y=\&quot;325\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-13\&quot; value=\&quot;Historical API\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;209\&quot; y=\&quot;310\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-17\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-15\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;667\&quot; y=\&quot;245\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-15\&quot; value=\&quot;Send Request to Backend\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;539\&quot; y=\&quot;230\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-20\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-19\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;727\&quot; y=\&quot;310\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-19\&quot; value=\&quot;Backend pulls weather data from GOV&amp;amp;nbsp;\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;672\&quot; y=\&quot;220\&quot; width=\&quot;110\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-21\&quot; value=\&quot;Fetch request displays data on frontend\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;672\&quot; y=\&quot;310\&quot; width=\&quot;112.5\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-25\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-23\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;726.5\&quot; y=\&quot;480\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-23\&quot; value=\&quot;Pulls .mp4 clips from bordertraffic.com&amp;amp;nbsp;\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;671.5\&quot; y=\&quot;390\&quot; width=\&quot;110\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-27\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-26\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;729.25\&quot; y=\&quot;550\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-26\&quot; value=\&quot;Uses pytz to localize timestamps to PST&amp;amp;nbsp;\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;671.5\&quot; y=\&quot;480\&quot; width=\&quot;115.5\&quot; height=\&quot;40\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-29\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;585\&quot; y=\&quot;589\&quot; as=\&quot;targetPoint\&quot; /&gt;\n            &lt;mxPoint x=\&quot;764.5\&quot; y=\&quot;589\&quot; as=\&quot;sourcePoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-28\&quot; value=\&quot;Includes backfill logic to download past 2hrs if no files exist on launch\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;666.5\&quot; y=\&quot;560\&quot; width=\&quot;125.5\&quot; height=\&quot;60\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-30\&quot; value=\&quot;Fetch request displays videos on frontend\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;460\&quot; y=\&quot;565\&quot; width=\&quot;120\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-43\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-32\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;280\&quot; y=\&quot;470\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-32\&quot; value=\&quot;timelapse.py\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;232.5\&quot; y=\&quot;400\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-44\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-34\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;280\&quot; y=\&quot;550\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-34\&quot; value=\&quot;moviepy for mp4 composition\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;230\&quot; y=\&quot;480\&quot; width=\&quot;100\&quot; height=\&quot;40\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-36\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-35\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;660\&quot; y=\&quot;415\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-35\&quot; value=\&quot;video_crawler.py\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;539\&quot; y=\&quot;400\&quot; width=\&quot;95\&quot; height=\&quot;30\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-39\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;451\&quot; y=\&quot;590\&quot; as=\&quot;targetPoint\&quot; /&gt;\n            &lt;mxPoint x=\&quot;323.5\&quot; y=\&quot;590\&quot; as=\&quot;sourcePoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-38\&quot; value=\&quot;Organized into timestamps for clarity\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;225\&quot; y=\&quot;562.5\&quot; width=\&quot;110\&quot; height=\&quot;55\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-47\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-46\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;100\&quot; y=\&quot;260\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-46\&quot; value=\&quot;uses csv file of long_term historical data of border crossing times\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;40\&quot; y=\&quot;290\&quot; width=\&quot;120\&quot; height=\&quot;70\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-51\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-50\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;100\&quot; y=\&quot;170\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-50\&quot; value=\&quot;Clean mapping of JSON to pandas DataFrame\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;46.25\&quot; y=\&quot;200\&quot; width=\&quot;107.5\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-58\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-52\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;200\&quot; y=\&quot;130\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-52\&quot; value=\&quot;Interactive Plotly visual with hover templates, line graphs, and annotations\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;36.25\&quot; y=\&quot;100\&quot; width=\&quot;127.5\&quot; height=\&quot;60\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-59\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-56\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;268.125\&quot; y=\&quot;190\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-56\&quot; value=\&quot;Used color and hover cues to focus on congestion trends\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;206.25\&quot; y=\&quot;105\&quot; width=\&quot;123.75\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-60\&quot; value=\&quot;Returned as HTML via Flask `Response`\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#f8cecc;strokeColor=#b85450;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;210\&quot; y=\&quot;200\&quot; width=\&quot;117.5\&quot; height=\&quot;50\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-64\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-63\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;427.5\&quot; y=\&quot;90\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-63\&quot; value=\&quot;Dual-mode support (`long_term` and `today`)\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;370.75\&quot; y=\&quot;120\&quot; width=\&quot;113.5\&quot; height=\&quot;60\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-66\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-65\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;580\&quot; y=\&quot;60\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-65\&quot; value=\&quot;Dynamic handling of missing inputs (`month`, `day`, `hour`) using `datetime`\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;307.5\&quot; y=\&quot;40\&quot; width=\&quot;240\&quot; height=\&quot;40\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-69\&quot; style=\&quot;edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;\&quot; parent=\&quot;1\&quot; source=\&quot;xbDnal-r1YM65dO4OVYU-68\&quot; edge=\&quot;1\&quot;&gt;\n          &lt;mxGeometry relative=\&quot;1\&quot; as=\&quot;geometry\&quot;&gt;\n            &lt;mxPoint x=\&quot;680\&quot; y=\&quot;130\&quot; as=\&quot;targetPoint\&quot; /&gt;\n          &lt;/mxGeometry&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-68\&quot; value=\&quot;Custom weighted average algorithm that compares CBP real-time data to historical averages\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;590\&quot; y=\&quot;25\&quot; width=\&quot;180\&quot; height=\&quot;70\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n        &lt;mxCell id=\&quot;xbDnal-r1YM65dO4OVYU-70\&quot; value=\&quot;Fetch request displays the estimated wait time for San Ysidro and Otay Mesa\&quot; style=\&quot;rounded=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;\&quot; parent=\&quot;1\&quot; vertex=\&quot;1\&quot;&gt;\n          &lt;mxGeometry x=\&quot;601.63\&quot; y=\&quot;140\&quot; width=\&quot;156.75\&quot; height=\&quot;60\&quot; as=\&quot;geometry\&quot; /&gt;\n        &lt;/mxCell&gt;\n      &lt;/root&gt;\n    &lt;/mxGraphModel&gt;\n  &lt;/diagram&gt;\n&lt;/mxfile&gt;\n&quot;}"></div>
<script type="text/javascript" src="https://viewer.diagrams.net/js/viewer-static.min.js"></script>
    
  <section class="bg-dark rounded-lg p-8 shadow-lg" id="table-of-contents">
    <h2 class="text-2xl font-bold text-accent mb-4">API Components Overview</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <a href="#prediction-api" class="text-gray-200 hover:text-accent">1. Intelligent Wait Time Prediction API</a>
      <a href="#visualization-api" class="text-gray-200 hover:text-accent">2. Historical Visualization API</a>
      <a href="#social-monitoring" class="text-gray-200 hover:text-accent">3. Live Social Media Monitoring</a>
      <a href="#facial-recognition" class="text-gray-200 hover:text-accent">4. Facial Recognition Utility</a>
      <a href="#weather-helper" class="text-gray-200 hover:text-accent">5. Weather Normalization Helper</a>
      <a href="#timelapse-generator" class="text-gray-200 hover:text-accent">6. Timelapse Video Generator</a>
      <a href="#feedback-collector" class="text-gray-200 hover:text-accent">7. Border Feedback Collector</a>
      <a href="#video-crawler" class="text-gray-200 hover:text-accent">8. Automated Border Video Crawler</a>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="prediction-api">
    <h2 class="text-2xl font-bold text-accent mb-4">1. Intelligent Wait Time Prediction API</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: border.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Designed a smart prediction API that uses both real-time scraping and ML-based long-term forecasting to return expected border wait times.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Provides highly relevant, accurate crossing time estimates for users planning trips.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Dual-mode support for both <code class="bg-gray-800 px-2 py-1 rounded">long_term</code> and <code class="bg-gray-800 px-2 py-1 rounded">today</code> predictions</li>
          <li>Dynamic handling of missing inputs (<code class="bg-gray-800 px-2 py-1 rounded">month</code>, <code class="bg-gray-800 px-2 py-1 rounded">day</code>, <code class="bg-gray-800 px-2 py-1 rounded">hour</code>) using <code class="bg-gray-800 px-2 py-1 rounded">datetime</code></li>
          <li>Custom weighted average algorithm that compares CBP real-time data to historical averages</li>
          <li>Intelligent fallback mechanisms for data unavailability scenarios</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="visualization-api">
    <h2 class="text-2xl font-bold text-accent mb-4">2. Historical Visualization API with Plotly</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: historicalgraph_api.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Built a visual API endpoint that returns an interactive Plotly chart displaying average hourly wait times across weekdays.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Helps users and analysts find patterns in border congestion throughout the week.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Clean mapping of JSON data to pandas DataFrame for efficient processing</li>
          <li>Interactive Plotly visualizations with hover templates, line graphs, and annotations</li>
          <li>Advanced color coding and hover cues to focus on congestion trends</li>
          <li>Seamless HTML output via Flask <code class="bg-gray-800 px-2 py-1 rounded">Response</code> object</li>
          <li>Responsive design that adapts to different screen sizes</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="social-monitoring">
    <h2 class="text-2xl font-bold text-accent mb-4">3. Live Social Media Monitoring</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">Files: twitter.py, twitter_search.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Implemented a Twitter-based keyword listener that extracts tweets about border delays and incidents.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Augments our data model with real user reports on unusual delays, accidents, or alerts from the border community.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Sophisticated query construction using geotagged search for the border region</li>
          <li>Secure integration with Twitter Bearer Token authentication</li>
          <li>Pluggable architecture via <code class="bg-gray-800 px-2 py-1 rounded">run_border_queries()</code> in main runtime</li>
          <li>Real-time sentiment analysis and keyword filtering</li>
          <li>Automated anomaly detection for unusual border events</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="facial-recognition">
    <h2 class="text-2xl font-bold text-accent mb-4">4. Facial Recognition Encoding Utility</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: facial_encoding.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Built a utility using the <code class="bg-gray-800 px-2 py-1 rounded">face_recognition</code> library to generate secure encodings from user-submitted images.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Enables future authentication or personalization features while maintaining user privacy and security.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Advanced face landmark detection and feature extraction</li>
          <li>Secure encoding storage in a consistent, encrypted format</li>
          <li>Modular utility design for easy expansion and integration</li>
          <li>Privacy-first approach with no raw image storage</li>
          <li>Error handling for various image formats and quality levels</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="weather-helper">
    <h2 class="text-2xl font-bold text-accent mb-4">5. Weather Normalization Helper</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: weather_formater.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Converts raw weather data into structured summaries with icons and descriptive text.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Supports context-aware guidance such as "Expect longer delays during fog" or "Clear weather - normal wait times expected."
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Comprehensive mapping of weather codes to descriptive conditions</li>
          <li>Clean separation of formatting logic for optimized API consumption</li>
          <li>Multi-language support for weather descriptions</li>
          <li>Integration with border wait time correlation algorithms</li>
          <li>Automated weather impact assessment on crossing conditions</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="timelapse-generator">
    <h2 class="text-2xl font-bold text-accent mb-4">6. Timelapse Video Generator (Traffic Review)</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: timelapse.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Generated stitched video summaries using saved traffic cam footage throughout a day.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Allows users to visually review congestion patterns before choosing optimal crossing times.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Efficient use of <code class="bg-gray-800 px-2 py-1 rounded">moviepy</code> for MP4 composition and rendering</li>
          <li>Organized file structure with timestamped folders for easy navigation</li>
          <li>Automated video quality optimization for web delivery</li>
          <li>Customizable playback speeds and time intervals</li>
          <li>Integration with historical wait time data overlay</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="feedback-collector">
    <h2 class="text-2xl font-bold text-accent mb-4">7. Structured Border Feedback Collector</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: border_feedback.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Created a comprehensive feedback API to gather user reports on real-life wait experiences.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Trains and improves our long-term prediction models using community-submitted data and real user experiences.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Robust validation for email, rating, and location fields</li>
          <li>Automated timestamp generation and secure data storage</li>
          <li>Integration with machine learning training pipelines</li>
          <li>Anonymous feedback options for privacy-conscious users</li>
          <li>Real-time feedback analysis for immediate system improvements</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="video-crawler">
    <h2 class="text-2xl font-bold text-accent mb-4">8. Automated Border Video Crawler</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: video_crawler.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Developed a sophisticated background script that crawls and downloads time-stamped traffic cam footage from the San Ysidro crossing every 29 seconds.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Supports timelapse generation and historical visual analysis of real border wait conditions throughout the day.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Automated pulling of <code class="bg-gray-800 px-2 py-1 rounded">.mp4</code> clips from <code class="bg-gray-800 px-2 py-1 rounded">bordertraffic.com</code> based on UTC-formatted filenames</li>
          <li>Advanced use of <code class="bg-gray-800 px-2 py-1 rounded">pytz</code> to localize timestamps to Pacific Time</li>
          <li>Intelligent backfill logic to download the past 2 hours of footage if no files exist on launch</li>
          <li>Comprehensive error handling for unavailable videos and server timeouts</li>
          <li>Retry mechanisms with exponential backoff for network resilience</li>
          <li>Efficient storage management with automatic cleanup of old footage</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="system-overview">
    <h2 class="text-2xl font-bold text-accent mb-4">System Architecture Overview</h2>
    
    <p class="text-gray-200 mb-6">
      Together, these components demonstrate a comprehensive approach to border crossing prediction and management:
    </p>
    
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Full-Stack Engineering</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>RESTful APIs with comprehensive documentation</li>
          <li>Advanced data models and database optimization</li>
          <li>Interactive visualization components</li>
          <li>Utility scripts for automation and maintenance</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">ML + Real-time Forecasting</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>Machine learning algorithms for pattern recognition</li>
          <li>Real-time data integration and processing</li>
          <li>Predictive modeling with continuous improvement</li>
          <li>Multi-source data fusion for accuracy</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Usability and Reliability</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>User-centered design principles</li>
          <li>Robust error handling and fallback mechanisms</li>
          <li>Performance optimization and caching strategies</li>
          <li>Comprehensive testing and monitoring</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Scalability and Security</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>Modular architecture for easy expansion</li>
          <li>Secure data handling and privacy protection</li>
          <li>API rate limiting and authentication</li>
          <li>Cloud-ready deployment strategies</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg">
    <div class="mt-8 p-4 border border-gray-700 rounded-md text-center">
      <p class="text-gray-300">
        This API documentation represents the technical foundation of CrossWise Smart Guide's intelligent border crossing prediction system. Each component is designed for reliability, scalability, and continuous improvement.
      </p>
      <p class="text-gray-400 mt-4 text-sm italic">
        For technical support or integration questions, please contact our development team. All APIs include comprehensive error handling and detailed logging for debugging and monitoring purposes.
      </p>
    </div>
  </section>
</div>
