# Discord Sunucu Koruyucu

Discord sunucularında hassas bilgilerin metin kanallarında paylaşılmamasını sağlamak için kullanabileceğiniz bir Regex tabanlı koruma sistemidir.

![image](https://github.com/kadinkatilii/Discord-Tc-Onleyici/assets/136261711/83c4ec88-39a5-4575-8dbd-ddb935ce96ee)


![image](https://github.com/kadinkatilii/Discord-Tc-Onleyici/assets/136261711/b75c7c7c-5f5f-4270-9e2a-963708137198)


![image](https://github.com/kadinkatilii/Discord-Tc-Onleyici/assets/136261711/e62eb305-4f0d-4dab-bdf2-853189f8161f)

## Kurulum

AutoMod eklentisine aşağıdaki regex kodlarını ekleyin:

## Regexler

Aşağıda listelenen regex kodları farklı veri tiplerini korumak için kullanılabilir:

### Cep Telefonu Numarası

- Kabul edilen formatlar: 05231231212, 0523 123 12 12
- Regex: `/^(05)([0-9]{2})\s?([0-9]{3})\s?([0-9]{2})\s?([0-9]{2})$/`

### Sabit Telefonu Numarası

- Kabul edilen formatlar: 02231231212, 0223 123 12 12
- Regex: `/^(0)([2348]{1})([0-9]{2})\s?([0-9]{3})\s?([0-9]{2})\s?([0-9]{2})$/`

### TC Kimlik Numarası

- Kabul edilen formatlar: 12345678902, 12345678900
- Regex: `/^[1-9]{1}[0-9]{9}[02468]{1}$/`

### Vergi Numarası

- Kabul edilen formatlar: 1234567890
- Regex: `/^[0-9]{10}$/`

### Kredi Kartı Numarası

- Kabul edilen formatlar: 1111222233334444, 1111 2222 3333 4444
- Regex: `/^([0-9]{4})\s?([0-9]{4})\s?([0-9]{4})\s?([0-9]{4})$/`

### Araç Plakası

- Kabul edilen formatlar: 34A2344, 34A23415, 06BK123, 06JK1234, 81ABC75
- Regex: `/^(0[1-9]|[1-7][0-9]|8[01])(([A-Z])(\d{4,5})|([A-Z]{2})(\d{3,4})|([A-Z]{3})(\d{2,3}))$/`

### Doğum Tarihi

- Kabul edilen formatlar: 13.08.1987, 13081987, 13/08/1987, 13-08-1987, 13 08 1987
- Regex: `/^([1-9]|[12][0-9]|3[01])(|\/|\.|\-|\s)?(0[1-9]|1[12])\2(19[0-9]{2}|200[0-9]|201[0-8])$/`
