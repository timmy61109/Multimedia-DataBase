#多媒體資料庫
參照Git運作方式，但不會一樣，但希望可以直接引用Git去執行這個，但修改部份功能，會用Python做運作的方式，可以利用Python產生對應的資料。而鍵值對應檔案的資料表會被Git所版本管控，而影片不會被加入到版本管理因此加速管理影片的效率。

## 目錄結構
###資料庫結構

```
__mmdb__ --- table --- table name.yaml --- file hash
          |                             |- file name
          |                             |- feature hash
          |- object --- multimedia object
                     |- info object
                     |- feature object
```

### 暫存目錄結構

```
__mpdlcache__
```

## 資料庫功能
多媒體資料庫的控制模組，以提供簡單功能:

- 運作:可利用Python函式與套件去呼叫與執行套件。
- 佈署:可利用Python函式與套件去呼叫與執行套件去建立新的資料庫。
- 資料儲存:儲存匯入進來的多媒體，可以指定檔案、目錄或者暫存。
- 資料管理:管理資料庫裡面的內容，操作基本的新增、刪除、修改與查詢。

並提供簡單資料庫操作方式:

- 新增:新增資料庫。
- 刪除:刪除資料庫。
- 修改:修改資料庫名稱。
- 查詢:提供迴遞的方式掃描所有目錄底下是否有資料庫。

並提供簡單資料表操作方式:

- 新增:新增資料表。
- 刪除:刪除資料表。
- 修改:修改資料表名稱。
- 查詢:查詢資料庫內線有的資料表。

並提供簡單資料操作方式:

- 新增:新增多媒體到資料庫裡面，並將資料紀錄在資料表上。
- 刪除:從資料庫裡面刪除資料，並提供刪除參照或物件的選項。
- 修改:更新資料庫裡面的資料，提供更新資料、多媒體、物件與參照。
- 查詢:查詢資料庫內容，並且依需求將資料匯出。
