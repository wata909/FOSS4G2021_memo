# FOSS4G2021_memo
FOSS4G2021の振り返りメモ

## Community / OSGeo
### [ The secret life of open source developers](https://callforpapers.2021.foss4g.org/foss4g2021/talk/VCGQZX/)[Video](https://www.youtube.com/watch?v=xDGn6FnPkps)

### [The Intersection of Geospatial Open Source and Commerce](https://callforpapers.2021.foss4g.org/foss4g2021/talk/ERGXPC/)  
[video](https://www.youtube.com/watch?v=2_EKhNNaeyQ)
-  This talk aims to describe several of the different paths that commercial organizations take to leverage free and open technologies for business success.The following three real world examples will illustrate these paths:  
    1. Very small organizations providing FOSS4G consulting and training services
    1. Product companies including FOSS4G tools in powering niche products
    1. Platform companies that have built their platforms upon open source frameworks
- The case study examples will include further details including how my current employer utilizes open source technology. Finally, the talk will speculate on why large, commercial companies such as Google, routinely open source their own technologies such as Kubernetes and other geospatial examples.
- This presentation looks plainly at the business aspects of the FOSS4G ecosystem. In short, how does free and open source software for geospatial help cultivate business success and sustain livelihoods?

## Client Side
### [OSGeo in the browser: Advances in client-side WebAssembly-based Geospatial Analysis and frontend visualization using jsgeoda and Vis.gl ](https://callforpapers.2021.foss4g.org/foss4g2021/talk/VESZRE/) 
[Link to Video](https://www.youtube.com/watch?v=FnTZrOrQL-s)
- In-browser analytics have grown in popularity as personal computers and mobile devices have increased capabilities in CPU and GPU performance to handle and represent geospatial data. Efficient data transfer formats, in-memory analytics, and cheap static or serverless web infrastructures set the groundwork for robust client-side data handling, parsing, and visualization. Additionally, the ongoing development of WebAssembly libraries, a web technology to wrap and translate existing modules from C, Go, Rust, Python, Java, etc. into a JavaScript virtual machine with near-native performance, opens the door to integrate existing work into new web applications. 
    > - ブラウザ内分析は、パーソナルコンピュータとモバイルデバイスがCPUとGPUによりパフォーマンスが向上したため、空間データを処理して表現するために人気が高まっている。効率的なデータ転送フォーマット、インメモリ分析、安価な静的またはサーバレスのWebインフラストラクチャは、堅牢なクライアントサイドのデータ処理、解析、視覚化の基礎となる。さらに、C、Go、Rust、Python、Javaなどの既存のモジュールを、ネイティブに近いパフォーマンスを持つJavaScript仮想マシンにラップして変換するWebテクノロジであるWebAssemblyライブラリの継続的な開発により、既存の作業を新しいWebアプリケーションに統合する道が開かれている。

- In response to the COVID-19 pandemic, a research coalition led by the Center for Spatial Data Science at UChicago developed a first-of-its-kind dashboard that enables client-side analytics to perform spatial autocorrelation methods (LISA / Local Moran’s I) and binning algorithms including jenks natural breaks and hinge breaks directly in the client-side environment. The advances open up new possibilities for inexpensively hosted geospatial web applications with more robust analytic capacities than previously possible, all while utilizing free or low-cost web hosting services. Additionally, new visualization methods utilizing powerful WebGL-based geospatial libraries (Deck.gl, Kepler.gl) allow for more complex on-the-fly visualizations such as point-grid layers and dot density maps with robust filtering options.
    > - COVID-19の世界的流行に対応して、UChicagoのCenter for Spatial Data Scienceが主導する研究連合は、クライアントサイド分析が空間的自動相関法(LISA/Local Moran's I)と、ジェンクス自然分裂やヒンジ分裂を含むビニングアルゴリズムをクライアントサイド環境で直接実行できるようにする、初めてのダッシュボードを開発した。この進歩により、無料または低コストのWebホスティングサービスを利用しながら、従来よりも堅牢な分析能力を備えた、安価にホストされる地理空間Webアプリケーションの新たな可能性が開かれます。さらに、強力なWebGLベースの地理空間ライブラリ(Deck.gl、Kepler.gl)を使用する新しい視覚化メソッドにより、堅牢なフィルタリングオプションを備えたポイントグリッドレイヤやドット密度マップなど、より複雑なオンザフライ視覚化が可能になります。

- This talk outlines the infrastructure used in the US Covid Atlas project and the capacities of jsgeoda (Xun Li, CSDS) to perform a variety of clustering and binning algorithms in the browser. Code demonstrations for main thread and worker implementations will be presented, along with a series of template Github repositories available for use licensed under GPL. By the end of this talk, viewers will be able to understand and replicate the US Covid Atlas’s web infrastructure, implement a simple jsgeoda instance for spatial clustering, and build from open source templates for their own geospatial analytics web application that does not require backend services.
    > - この講演では、米国のCovid Atlasプロジェクトで使用されているインフラストラクチャと、ブラウザでさまざまなクラスタリングとビニングアルゴリズムを実行するjsgeoda(詢Li,CSDS)の能力について概説する。メインスレッドとワーカー実装のコードデモと、GPLの下でライセンスされた使用可能な一連のテンプレートGithubリポジトリを提示する。この講演の終わりまでに、視聴者は、米国のCovid AtlasのWebインフラストラクチャを理解して複製し、空間クラスタリングのためのシンプルなjsgeodaインスタンスを実装し、バックエンドサービスを必要としない独自の空間分析Webアプリケーション用のオープンソーステンプレートから構築することができるようになるだろう。

### [Browser-side geoprocessing with Turf.js and Leaflet ](https://callforpapers.2021.foss4g.org/foss4g2021/talk/AFMPSV/)
 [Video](https://www.youtube.com/watch?v=mS-o7UGSRu8)
- This workshop teaches how to use the JavaScript library Turf.js to execute client-side geoprocessing tasks. Browser-side geoprocessing is an alternative to using Web Processing Services (WPS), which require a complex server-side infrastructure and which take longer to return results, even for trivial tasks, and whose setup requires a considerable set of skills and necessary user permissions. Turf.js is a pure JavaScript library, meaning that anyone with a basic knowledge of JavaScript can get started quickly. Turf.js is very well documented, flexible, and user friendly. It offers a multitude of geoprocessing tools, covering all the classics that are used in every desktop GIS software (e.g., buffer, erase, intersect, merge) and many advanced features.

During the workshop a variety of examples, as well as live coding, are shown using Leaflet as a mapping client, but participants will also be shown how to use Turf.js with OpenLayers. Participants will first be taught how to set up a simple map and then will be walked through preparing datasets from various formats (e.g., KML, GPX, Shapefile), so they can be used with Turf.js, which requires GeoJSON as input. This will be followed by the presentation of various tools, as well as the combination of them, to conduct meaningful geospatial analysis and queries, whose results can be displayed and exported.

This workshop is taught by the author of the Leaflet Cookbook - Recipes for Creating Dynamic Web Maps (Locate Press, 2019).

Web development knowledge is a benefit, but not a necessity. The workshop will focus on Turf and anything related to general web dev of Leaflet will be explicitly mentioned and explained, if need be. All data, code, and outcomes will be shared. Feel free to simply sit back and enjoy! If you want to follow along, all you need is a simple text editor (or your IDE of choice). I will show how to convert various vector formats to GeoJSON using QGIS. If you don’t have QGIS I can share the outcomes with you (but you should nevertheless probably get QGIS, because it’s a really, really good product :-)).

### [Handling GeoTIFFs in client-side code with GDAL and Loam](https://callforpapers.2021.foss4g.org/foss4g2021/talk/NZYLKZ/)
[Video](https://www.youtube.com/watch?v=WYQH7AWViCo)
- GDAL provides extensive capabilities for processing GeoTIFFs and other spatial data formats. However, until recently, the use of GDAL in web applications was limited to server-side code. This talk will describe how we use WebAssembly and a new wrapper library we developed, called Loam, to make GDAL's suite of tools accessible from client-side code. This strategy enables improved user experiences and can lower infrastructure costs for web applications handling GeoTIFFs and other spatial data.

### [Live coding: WebGL shaders, rasters and symbols](https://callforpapers.2021.foss4g.org/foss4g2021/talk/CGTLWC/)
- [video](https://www.youtube.com/watch?v=zX8fBQiR-2Q)
- A live coding session on WebGL graphics manipulation: abstract shaders, pixel manipulation on multisample rasters, and "classic" GIS map symbols.

### [Techniques for representing untiled GIS data in WebGL structures](https://callforpapers.2021.foss4g.org/foss4g2021/talk/AACZSH/index.html)
- [video](https://www.youtube.com/watch?v=HX-Wz3O3Cgo)
- WebGL allows for fast graphics rendering on most web browsers, but also inherits undesired traits from from its videogame legacy. One of these traits is low numerical precision on integer and floating point operations.
- Tiling datasets has allowed tiles (both raster and vector) to dominate web applications since tiles can easily overcome these problems. This talk will explore the opposite: possible ways to overcome numerical precision challenges in untiled datasets, as well as the dreaded antimeridian artefacts in coordinate systems which wrap around the globe.

<!-- ここまでClient Side -->

## SaaS, Server, Cloud Optimize
<!-- Google Earth Engin とか、サーバレストか、Cloud optimizeフォーマット系の情報 -->
### [An Open Data Cube Sandbox using Google Colab](https://callforpapers.2021.foss4g.org/foss4g2021/talk/JQSTJT/)
- The Open Data Cube (ODC) Google Sandbox is a free and open programming interface that connects users to Google Earth Engine datasets. 

### [PMTiles: An open, cloud-optimized archive format for serverless map data](https://callforpapers.2021.foss4g.org/foss4g2021/talk/TN8QTW/)
[video](https://www.youtube.com/watch?v=0pFvc_q_SV4)
- Have you ever wished for web maps with no servers or backend to maintain? Introducing a new archive format called PMTiles, based on HTTP Range requests, for serving Z/X/Y tiles from storage APIs such as S3.

### [Cloud optimized formats for rasters and vectors explained](https://callforpapers.2021.foss4g.org/foss4g2021/talk/ZJYRAS/)
- [video](https://www.youtube.com/watch?v=hnWkbMBdhyg)
- Cloud Optimized GeoTIFF (COG) and FlatGeobuf support efficient access to raster and vector data using the HTTP protocol. This talk explains how this works behind the scenes (hint: HTTP GET range requests) and what this means for efficient use of these formats.

### [Building Serverless Geospatial Applications for the Enterprise](https://callforpapers.2021.foss4g.org/foss4g2021/talk/CVNDST/)
- [video](https://www.youtube.com/watch?v=AvxQM1cDIuw)
- This presentation will provide an overview of how to leverage common cloud services to develop serverless applications and a synopsis of several case studies where this approach facilitated delivery of more sustainable dynamic geospatial analytics and interoperability solutions.
    - Topic – New trends: IoT, Indoor mapping, drones - UAV (unmanned aerial vehicle), Artificial intelligence - machine learning, deep learning-, geospatial data structures, real time raster analysis

<!-- ここまでGoogle Earth Engin とか、サーバレストか、Cloud optimizeフォーマット系の情報 -->

## Use case
### [Cold war reconnaissance imagery reloaded: orthorectifying the 1960s in high resolution](https://callforpapers.2021.foss4g.org/foss4g2021/talk/7ERWUY/)
- Coronaデータの活用方法  
    - Data は [USGS EROS Archive - Declassified Data - Declassified Satellite Imagery - 1 ](https://www.usgs.gov/centers/eros/science/usgs-eros-archive-declassified-data-declassified-satellite-imagery-1) からダウンロード可能か？

### [Land cover classification using freely available multitemporal SAR data (work in progress)](https://www.youtube.com/watch?v=HAbG79U3j78)
- [video](https://www.youtube.com/watch?v=HAbG79U3j78)
- In this work, we consider a portion of the Bajo Delta of the Paraná River, a wide coastal freshwater wetland located in Buenos Aires, Argentina. Due to the high amount of biomass in all its extent, mapping and monitoring this area is particularly challenging. The main objective of this work are:
    - to study the potential of multitemporal Sentinel-1 datasets for land cover maps in densely vegetated areas,
    - to classify the study area and compare the performance of the different multitemporal Sentinel-1 datasets.
- The Sentinel-1 images were processed using SNAP. The classification was done using Python (libraries: sklearn, pandas, numpy, and gdal).

### [Metadata Nirvana: Data discovery and metadata creation untouched by human hands](https://callforpapers.2021.foss4g.org/foss4g2021/talk/HACU98/)
- [video](https://www.youtube.com/watch?v=sw30nuzmb3A)
- Everyone knows metadata is A Good Idea and Very Important, even more so given the current focus on data sharing. Unfortunately it's also time-consuming, hard work, and a bit boring. Assuming you've even kept tags on all of your data sources, manual metadata creation also doesn't work well at scale.
- Out of date, inaccurate, or incomplete metadata can lead to bad decision-making with real-world consequences. Conversely, good metadata can help make your data far more discoverable on the web.
What if you could automatically keep track of all your geospatial data, create fully valid, high-quality metadata records, including the fluffy stuff such as abstracts and keywords, and keep it up to date?
- I'll demonstrate a potential workflow for reaching metadata nirvana using entirely open source tools such as GeoNetwork, Talend ETL, and some Natural Language Processing libraries. While the underlying subject is complex, the talk will be pitched at an accessible level.

## GPU
### [FOSS4GPU: Faster GIS via GPU and cuSpatial](https://callforpapers.2021.foss4g.org/foss4g2021/talk/BF8AWV/)  
[Video](https://www.youtube.com/watch?v=8psWMdgWKkA)
- cuSpatial is a FOSS library for accelerating spatial workflows on the GPU.
- cuSpatial is in development and enables GPU acceleration for a number of common GIS workflows including:
    - GeoPandas integration
    - fast I/O with Apache Arrow and Apache Parquet
    - point-in-polygon
    - cubic spline fitting
    - hausdorff-distance based clustering
    - haversine distance and geographic to euclidean projection

## 注
翻訳は、[みんなの自動翻訳](https://mt-auto-minhon-mlt.ucri.jgn-x.jp/)にて実施。