<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · hi · no clinical/professional/rights approval -->

# METs से ऊर्जा व्यय

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/gasto-energetico-por-mets)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### गतिविधि की तीव्रता (Compendium का मान)

`met`

METs · सीमा: 1–25

### वज़न

`peso`

kg · सीमा: 20–300

### सत्र की अवधि

`min`

min · सीमा: 1–600

### प्रति सप्ताह सत्र

`sessoes`

वैकल्पिक · सीमा: 1–14

## विधि का संस्करण

मानक MET 3.5 mL O₂/kg/min; kcal/min=MET×3.5×kg/200; Compendium 2024 संदर्भ

## दस्तावेज़ित सूत्र

kcal/min = METs × 3.5 × वजन (kg) ÷ 200 (1 MET = 3.5 mL O2/kg/min; प्रति लीटर O2 लगभग 5 kcal)।

MET-min = METs × मिनट। समतुल्य सन्निकटन: kcal ≈ METs × वजन (kg) × घंटे।

## सीमाएँ और जनसमूह

2024 वयस्क संकलन के MET 19–59 वर्ष के वयस्कों की गतिविधियों से संबंधित हैं; इस संस्करण से ≥60 वर्ष के लोगों का डेटा बाहर रखा गया। मानकीकृत मान, जिनमें अनुमानित मान भी शामिल हैं, व्यक्तिगत ऊर्जा व्यय नहीं मापते। बच्चों, वृद्धों और विशेष नैदानिक स्थितियों में उन आबादियों के अनुकूल स्रोत तथा विधियाँ आवश्यक हैं।

## संदर्भ

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026
