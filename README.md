# DDD-2025-Group3
<html>
<h5> Drini Bejtaga / Walter De Nicola / Roberta Valli</h5>
<header> 
  <h1> Alien.AI
</h1>
</header>
  <article>
    <h1>Data Collection</h1>
   <ul> 
     <li> Where did you get your data from? [source/s link]
</li>
     <li> Where did you get your data from? [source/s link]</li>
     <li> What’s your data about? [describe] </li>
     <li> Who is/are the sources/creators of your data?
</li>
   </ul>
    <h1> Data Organisation </h1>
  <ul>
    <li> Have you combined data from different sources? How did you merge them? </li>
    <li> What columns are more relevant for your project?</li>
    <li> Have you used any AI-based tool to understand or manipulate your data? if yes, what and how? </li>
    <h1> Protocollo </h1>
		graph TB
    Topic["Topic: Alien Imagery Film vs AI"]
    
    RQ(["Research Question:<br/>How does visual comparison between<br/>film aliens and AI-generated aliens<br/>reveal analogies, differences and<br/>recurring patterns?"])
    
    Topic --> RQ
    
    A1{"Select 100<br/>film aliens"}
    RQ --> A1
    
    A2{"Scraping attempt<br/>SERPAPI + Python"}
    A1 --> A2
    
    A3{"Manual image<br/>collection"}
    A2 -.-> A3
    
    D1[("Film Aliens Dataset<br/>100 images")]
    A3 --> D1
    
    T1(("Claude 3.5 Sonnet"))
    D1 --> T1
    
    A4{"Morphological analysis<br/>with standardized prompt"}
    T1 --> A4
    
    D2[("Morphological<br/>Descriptions")]
    A4 --> D2
    
    T2(("Gemini"))
    D2 --> T2
    
    A5{"Generate 100<br/>AI prompts"}
    T2 --> A5
    
    D3[("AI Generation Prompts")]
    A5 --> D3
    
    A6{"Test different<br/>AI models"}
    D3 --> A6
    
    A7{"Generation with<br/>Imagen 4.0"}
    A6 -.-> A7
    
    D4[("AI-Generated Aliens<br/>100 images")]
    A7 --> D4
    
    T3(("YOLO"))
    D4 --> T3
    D1 --> T3
    
    A8{"Morphological<br/>decomposition<br/>cropping"}
    T3 --> A8
    
    C1[/Head/]
    C2[/Eyes/]
    C3[/Mouth/]
    C4[/Hands/]
    C5[/Body/]
    C6[/Feet/]
    C7[/Texture/]
    
    A8 --> C1
    A8 --> C2
    A8 --> C3
    A8 --> C4
    A8 --> C5
    A8 --> C6
    A8 --> C7
    
    D5[("Morphological Components<br/>~1200 images")]
    
    C1 --> D5
    C2 --> D5
    C3 --> D5
    C4 --> D5
    C5 --> D5
    C6 --> D5
    C7 --> D5
    
    A9{"Dataset construction"}
    D5 --> A9
    D2 --> A9
    
    D6[("Final Dataset:<br/>Originals + Crops +<br/>Descriptions + Metadata")]
    A9 --> D6
    
    A10{"Interface prototyping"}
    D6 --> A10
    
    VIZ["Interactive Interface:<br/>Film World vs AI World<br/>Sphere exploration"]
    A10 --> VIZ
    
    INSIGHT{{Insights:<br/>Visual patterns and<br/>morphological analogies}}
    VIZ --> INSIGHT
    
    classDef failed fill:#d3d3d3,stroke:#333,stroke-dasharray: 5 5
    class A2,A6 failed
  </article>
</html>
