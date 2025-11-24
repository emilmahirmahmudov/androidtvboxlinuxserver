Quraşdırma Addımları (Multitool Metodu)
RK322x qutuları üçün bu, Armbian-ı daxili yaddaşa (eMMC/NAND) quraşdırmaq üçün ən sabit yoldur.

A. Hazırlıq və Yükləmə
Tələb Olunanlar:

microSD Kart: Ən azı 8 GB, sürətli  bir kart və bağlantı üçün SDHC adapter

PC: Kartı yaza biləcəyiniz Windows və ya Linux kompüteri.

USB Kabeli: Bəzən Rockchip cihazları üçün USB A-dan USB A-ya (Male-to-Male) kabel tələb olunur (bərpası üçün).

Flashing Proqramı: Məsələn, Balena Etcher.

İcma Resursları: https://forum.armbian.com/topic/34923-csc-armbian-for-rk322x-tv-box-boards/

Armbian sistemi img faylları : https://armbian.hosthatch.com/archive/rk322x-box/archive/

RK322x üçün rəsmi dəstək Armbian layihəsinin əsas depozitində deyil, icma tərəfindən dəstəklənən filialdadır. Ən son faylları və dəstəyi aşağıdakı Armbian Forumunda tapa bilərsiniz:

Armbian İcma Forumu (RK322x): CSC Armbian for RK322x TV box boards

Yüklənməli Fayllar:

Armbian Görüntüsü (.img.xz): Forum mövzusundan və ya Armbian-ın icma/gecəlik (nightly) yükləmə səhifəsindən rk322x-box hədəfi üçün Armbian görüntüsünü yükləyin.

Multitool Görüntüsü (multitool.img.xz): Bu, Armbian-ı daxili yaddaşa yazmaq üçün istifadə olunan xüsusi bir kiçik sistemdir. Bu faylı da yuxarıdakı icma mövzusundan yükləyin.

B. Multitool-un Hazırlanması
Multitool-u Kartaza Yazın:

Balena Etcher proqramını açın.

Mənbə kimi multitool.img.xz faylını seçin.

Hədəf kimi microSD kartınızı seçin və yazmağa başlayın (Flash).

Armbian Görüntüsünü Karta Köçürün:

Yazma prosesi bitdikdən sonra kartı çıxarın və yenidən PC-yə qoşun. Windows sizdən formatlamağı istəyə bilər, lakin bu təklifi rədd edin.

Kartda görünən FAT32 hissəsinə (adətən MULTI-TOOL adlanır) daxil olun.

Burada olan images qovluğuna yüklədiyiniz Armbian görüntüsünü (Armbian_xx.xx...rk322x-box...img.xz faylını) köçürün. Əksər hallarda, onu açmaq (extract etmək) lazım deyil.

C. Qutuya Yükləmə (Flashing)
SD Kartı Qutuya Daxil Edin: microSD kartı MXQ TV qutusunun kart yuvasına taxın.

Multitool-u Yükləyin (Boot):

TV qutusunun enerjisini kəsin.

Reset düyməsini (adətən AV girişində  yerləşir) nazik bir diş çöpü ilə basıb saxlayın.

Reset düyməsini basılı tutaraq qutuya enerji kabelini qoşun.

TV-də Multitool menyusu görünənə qədər Reset düyməsini bir neçə saniyə saxlayın.

Quraşdırma Əməliyyatları:

Multitool menyusunda klaviatura və ya pult vasitəsilə hərəkət edin.

(VACİB HİSSƏ) Backup: Əvvəlcə Android sisteminizin eMMC-də ehtiyat nüsxəsini çıxarmaq tövsiyə olunur.

eMMC Silinməsi (Önəmli): Armbian-ı təmiz quraşdırmaq üçün "Erase flash" və ya "Clear EMMC" seçimi ilə daxili yaddaşı silin.

Armbian-ı Quraşdırın: "Burn image to flash" (və ya oxşar) seçimini seçin.

Quraşdırılacaq hədəf cihazı (adətən mmcblk2 və ya rknand0) və images qovluğuna qoyduğunuz Armbian görüntüsünü seçin.

Prosesin tamamlanmasını gözləyin.

İlk Yükləmə:

Quraşdırma bitdikdən sonra SD kartı çıxarın.

Qutunu yenidən başladın (Reboot).

Qutu daxili yaddaşdan (eMMC) Armbian-ı yükləməlidir. İlk yükləmə bir neçə dəqiqə çəkə bilər.


Əgər SDHC dan sistem boot etmirsə məndə bu problemə yaşadım ilk öncə stock sistem qurraşdırın
Yuxarıda onun üçündə addımlar qeyd olunub.
