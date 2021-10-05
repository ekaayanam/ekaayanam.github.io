+++
title = "Computer setup"
unicode_script = "devanagari"
+++

## समानं कर्म
- अधः XYZ इति यद् अस्ति, तस्य स्थाने स्वीयं github-नाम प्रयुङ्क्ताम्।

## सङ्गणके समीचीनस्थानप्राप्तिः
- ततः समीचीनस्थाने terminal/ command-prompt इत्य् उद्घाट्य गच्छतु। यथा 
  - `cd F:\Git\` इति windows पक्षे
  - `cd ~` इति linux पक्षे

## सञ्चिकाप्राप्तिः
- सङ्गणके समीचीनस्थानप्राप्तिः इति भागे यद् उक्तं तत् कृत्वा

```
git clone --single-branch --depth 1 --branch master https://github.com/ekaayanam/ekaayanam.github.io.git ekaayanam-master
cd ekaayanam-master
git submodule update --init  themes/sanskrit-documentation-theme-hugo
cd ..

git clone --single-branch --depth 1 --branch content https://github.com/ekaayanam/ekaayanam.github.io.git ekaayanam-content
cd ekaayanam-content
git pull upstream content
cd ..
```

## hugo-चालनम्
- सङ्गणके समीचीन-स्थान-प्राप्तिः इति भागे यद् उक्तं तत् कृत्वा

```
cd ekaayanam-master
git pull upstream master
cd themes/sanskrit-documentation-theme-hugo/
git pull origin master
cd ../.. 
hugo server --renderToDisk --config ./config_dev.toml
```

## सञ्चिकासु प्राप्तासु सत्सु कार्यम्
- सङ्गणके समीचीन-स्थान-प्राप्तिः इति भागे यद् उक्तं तत् कृत्वा

```
cd ekaayanam-content
```

- यथापेक्षं सञ्चिकाः सम्पाद्य
- atom द्वारा वा github desktop द्वारा वा नुदेत् (commit, push इति कुर्यात्)।