# Sürüm Değişiklikleri

## Sürüm 2.0

### Yenilikler ve Değişiklikler

1. **Alt Görev Ekleme Özelliği**:
    - Görevlerin alt görevleri olabilir. Her görev için alt görevler eklenebilir, tamamlanabilir ve silinebilir.
    - Alt görevlerin durumu da tamamlanmış veya tamamlanmamış olarak ayarlanabilir.
    - Alt görevleri yönetmek için `add_subtask`, `complete_subtask`, ve `delete_subtask` fonksiyonları eklendi.
    - `update_subtask_list` fonksiyonu ile seçilen görevin alt görevleri güncellenir.

2. **Görev Düzenleme Özelliği**:
    - Mevcut görevler düzenlenebilir. Bunun için `edit_task` fonksiyonu eklendi.
    - Seçilen görev yeni bir görev metni ile güncellenir.

3. **Görev ve Alt Görevlerin Renkli Gösterimi**:
    - Tamamlanan görevler ve alt görevler yeşil, tamamlanmayanlar kırmızı renkte gösterilir.
    - `update_task_list` ve `update_subtask_list` fonksiyonları, görevlerin ve alt görevlerin renklerini ayarlar.

4. **Seçim İle Görev ve Alt Görev Yönetimi**:
    - Görevlerin ve alt görevlerin yönetimi için Listbox seçim özelliği kullanılır.
    - Görev ve alt görev seçimi ile ilgili işlemler, Listbox'tan seçilen öğeye göre yapılır.

5. **Yeni Widget'lar ve Düzenlemeler**:
    - `subtask_listbox` ve `subtask_entry` widget'ları eklendi.
    - `on_task_select` fonksiyonu ile bir görev seçildiğinde alt görevlerin güncellenmesi sağlandı.

### Kod Değişiklikleri

#### Eklenen Fonksiyonlar
- `add_subtask()`
- `complete_subtask()`
- `delete_subtask()`
- `edit_task()`
- `update_subtask_list()`

#### Güncellenen Fonksiyonlar
- `add_task()`
- `update_task_list()`
- `complete_task()`
- `delete_task()`

#### Yeni Widget'lar
- `subtask_listbox`
- `subtask_entry`
- `add_subtask_button`
- `complete_subtask_button`
- `delete_subtask_button`

#### Diğer Değişiklikler
- Görev ve alt görevler için renk ayarlamaları.
- Listbox seçim özelliği ile görev ve alt görev yönetimi.

### Sürüm 1.0 ile Sürüm 2.0 Arasındaki Farklar

- **Sürüm 1.0**: Temel görev ekleme, tamamlama ve silme özellikleri.
- **Sürüm 2.0**: Alt görev yönetimi, görev düzenleme, renkli gösterim ve gelişmiş kullanıcı arayüzü özellikleri.

