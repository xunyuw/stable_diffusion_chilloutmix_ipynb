# Prompts Collections - 标签集合

先介绍两种标签：

- **SFW**: Safe For Work - 较为安全
- **NSFW**: Not Safe For Work - **不安全 请勿在有客人的地方打开此类图片**

此处的标签大部分为 `SFW` 标签，但是在反向标签中有部分 SFW 没有加入反nsfw标签。

生成的图部分情况容易出现脸部瑕疵，出现手脚大问题需要另外再加入合适的反向标签，无法完全遏制出现错误的手脚

## 合集目录

- [\[SFW\] Cat ears + Blue eyes](#sfw-cat-ears--blue-eyes)
- [[SFW\] Blue long hair + Silver dress](#sfw-blue-long-hair--silver-dress)
- [\[SFW\] School uniform](#sfw-school-uniform)
- [\[SFW\] Side ponytail + Multicolored hair](#sfw-side-ponytail--multicolored-hair)
- [\[SFW\] Sleeveless white](#sfw-sleeveless-white)
- [\[SFW\] Redgown](#sfw-redgown)
- [\[NSFW?\] Seductive pose](#nsfw-seductive-pose)
- [\[SFW\] White sports bra + Outdoors](#sfw-white-sports-bra--outdoors)
- [\[SFW\] Blue long & elbow dress](#sfw-blue-long--elbow-dress)
- [\[SFW\] Platinum blonde hair + Black skirt](#sfw-platinum-blonde-hair--black-skirt)
- [\[SFW\] Black tight suit + Cyberpunk city](#sfw-black-tight-suit--cyberpunk-city)

## 作画小经验

- Lora _stLouisLuxuriousWheels_v1_ Weight = **1** - 即默认
- Lora _koreanDollLikeness_v10_ Weight = **0.5** - 多了有可能会引起面部扭曲，不止 koreanDollLikeness，其他类似的 Lora 都建议只开 0.5, 实在不行可以选择备用 **0.66**
- Sampler 选择 **DPM++ 2M Karras** 或者 **DPM++ SDE Karras**，个人使用 DPM++ 2M Karras 居多
- Steps 大多 **25** 步，这样的图会相对稳定
- CFG scale 一般为 **7**，部分时刻选择 **8** 但机会较少
- stLouisLuxuriousWheels 或 girlsFrontlineOts14 这一类**只开一个**就好，开多了有可能会导致画面混杂无章
- ChilloutMix 似乎画作的时候大部分都为 large breasts，因此必要的时候可以加入 `large breasts` 标签以抑制

## [SFW] Cat ears + Blue eyes

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219844710-25e94a0a-ad84-40b4-b5b7-703c03433b96.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1 white child, (ulzzang-6500:1.0), smiling, (PureErosFace_V1:1.0), ((detailed facial features)), alluring blue eyes, photographed on a Canon EOS R5, 50mm lens, F/2.8, HDR, 8k resolution, ulzzang-6500, (kpop idol), aegyo sal, from side, looking at camera, cat ears, sports bra,
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans
```

### Others 其他

- Steps: 25
- Sampler: DPM++ 2M Karras
- CFG scale: 7
- Size: 512x512
- Model: chilloutmix
- AddNet Enabled: True
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] Blue long hair + Silver dress


<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219844772-dc9a0217-0696-4bdc-8638-4dc3e8824570.png">
</details>


### Prompts 提示标签

```
best quality, blue long hair, ultra high res, (photorealistic:1.4), 1girl,silver dress
```

### Negative prompts 反向提示标签

```
EasyNegative, paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans,extra fingers,fewer fingers,
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] School uniform


<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219844868-3703c832-3db4-419d-b38e-f10346d802bf.png">
</details>


### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1girl,school uniform,cute,(platinum blonde grey hair:1), ((puffy eyes)), looking at viewer, full body
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw,
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] Side ponytail + Multicolored hair

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219844902-bfebdfe4-b1cc-4c40-8f75-9a87e9d93b66.png">
</details>


### Prompts 提示标签

```
side ponytail, ((nahida \(genshin impact\))), (((Kpop idol))),aegyo sal,multicolored hair,((hair between eyes)),white hair,green hair,green eyes,((pointy ears)),((flat chest)),(photorealistic:1.4),(masterpiece:1.4),(best quality:1.4),1girl, solo,ultra high res,((detailed facial features)),upper body, small hands,
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, (outdoor:1.6), manboobs, backlight,(ugly:1.331), (duplicate:1.331), (morbid:1.21), (mutilated:1.21), (tranny:1.331), mutated hands, (poorly drawn hands:1.331), blurry, (bad anatomy:1.21), (bad proportions:1.331), extra limbs, (disfigured:1.331), (more than 2 nipples:1.331), (missing arms:1.331), (extra legs:1.331), (fused fingers:1.61051), (too many fingers:1.61051), (unclear eyes:1.331), bad hands, missing fingers, extra digit, (futa:1.1), bad body, NG_DeepNegative_V1_75T,pubic hair, glans,(nipples:1.41),nsfw,
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] Sleeveless white

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219845586-353eb02f-be61-4801-b302-58ddec94e1b3.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1girl, sleeveless white , cute, (Kpop idol), (aegyo sal:1), (platinum blonde hair:1), ((puffy eyes)), looking at viewer, full body, facing front, smiling
```

### Negative prompts 反向提示标签

```
EasyNegative, paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans,extra fingers,fewer fingers,
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] Redgown

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219846183-813f3051-3dd3-4fad-bcbd-c258a47b572b.png">
</details>


### Prompts 提示标签

```
best quality, blonde hair, long hair, ultra high res, (photorealistic:1.4), 1girl, redgown, redhat,(upper body), (Kpop idol), (aegyo sal:1), (platinum blonde hair:1), ((puffy eyes)), looking at viewer, facing front, wet skin, rain, night,
```

### Negative prompts 反向提示标签

```
EasyNegative, paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, extra fingers, fewer fingers,watermark,
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: **girlsFrontlineOts14_v30(c2824b876e6b)**, AddNet Weight A 2: 1, AddNet Weight B 2: 1

## `[NSFW?]` Seductive pose

> 此 tag 有可能会诱发 NSFW (`large breasts` 标签)，建议使用的时候加入反nsfw类标签

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219846499-d02929d9-e332-40fb-93f0-92711460ab62.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1girl, white camisole, (Kpop idol), (aegyo sal:1), (seductive pose),(busty), (cleavage), (curvy), large breasts,(blonde grey long hair:1.3), (((looking at viewer))), ((full body)), ((puffy eyes)), ((closeup))
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 

## [SFW] White sports bra + Outdoors

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219847185-ab8638c5-7cba-4340-931d-4a8f73b2f34f.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1girl, loose and oversized black jacket, white sports bra, (green yoga pants:1), (Kpop idol), (aegyo sal:1), (light brown short ponytail:1.2), ((puffy eyes)), looking at viewer, smiling, cute, full body, streets, outdoors
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.65, AddNet Weight B 1: 0.5, 

## [SFW] Blue long & elbow dress

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219847968-28c4ce66-ee33-4007-9264-611e8fbb7738.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1girl, solo focus, ((blue long dress)), elbow dress, black thighhighs, frills, ribbons, studio background, (Kpop idol), (aegyo sal:1), (platinum blonde hair:1), ((puffy eyes)), looking at viewer, facing front, smiling, laughing
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw, nipples
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.65, AddNet Weight B 1: 0.5, 

## [SFW] Platinum blonde hair + Black skirt

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219868371-1278e017-f4ce-4751-b32a-f2a1daa754b3.png">
</details>

### Prompts 提示标签

```
best quality, ultra high res, (photorealistic:1.4), 1woman, sleeveless white button shirt, black skirt, black choker, cute, (Kpop idol), (aegyo sal:1), (platinum blonde hair:1), ((puffy eyes)), looking at viewer, full body, facing front, masterpiece, best quality,
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw, nipples, lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1

## [SFW] Black tight suit + Cyberpunk city

<details>
  <summary> <h3>Demo 案例</h3> </summary>
  <img width="350" src="https://user-images.githubusercontent.com/62133302/219876219-15425a3b-1f4a-4126-9bd5-71dd73eddc84.png">
</details>


### Prompts 提示标签

```
(8k, RAW photo, best quality, masterpiece:1.2), (realistic, photo-realistic:1.37),(Kpop idol), (aegyo sal:1),cute,professional lighting, photon mapping, radiosity, physically-based rendering, cosplay, lucy \(cyberpunk\),bob cut,mechanical parts,grey eyes, black tight suit,cyberpunk city, black pants,night,neon lights,sexy,porn,smoke, looking at viewer,
```

### Negative prompts 反向提示标签

```
paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans, nsfw, nipples, lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry
```

### Others 其他

- Steps: 25, 
- Sampler: DPM++ 2M Karras, 
- CFG scale: 7, 
- Model: chilloutmix, 
- AddNet Enabled: True, 
- AddNet Module 1: LoRA, AddNet Model 1: koreanDollLikeness_v10(e2e472c06607), AddNet Weight A 1: 0.5, AddNet Weight B 1: 0.5, 
- AddNet Module 2: LoRA, AddNet Model 2: stLouisLuxuriousWheels_v1(034b97419349), AddNet Weight A 2: 1, AddNet Weight B 2: 1