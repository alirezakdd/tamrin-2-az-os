

## 1:



```bash
mkdir -p project/assets/{css,pages,py}
```

```text
project/
└── assets/
    ├── css/
    ├── pages/
    └── py/
```

---

## 2:

### Step 1:

```bash
echo "Hey alireza" > info.txt
```

### Step 2: hardlink

```bash
ln info.txt info_hard
```

### Step 3: softink

```bash
ln -s info.txt info_soft
```

### Step 4: 

```bash
ls -li info.txt info_hard info_soft
```

### Step 5: Deleting

```bash
rm info.txt
```

### Step 6: 

```bash
cat info_hard
cat info_soft
```
### Result:

cat info_hard displays Hey alireza رو نشون میده چون هارد لینک همچنان به داده ی همون فایل اشاره میکنه.

cat info_soft ارور نشون میده چون مسیر فایل اصلی دیگه وجود نداره.


### conclusion:

هارد لینک به همون اینود فایل اصلی اشاره میکنه در حالی که سافت لینک مسیر فایل مقصد رو ذخیره میکنه
---

## 3: 

### Step 1:

```bash
man rm
```

### Step 2:

Press `/`, type `-f`,and enter. press `n` to find the next match.

### Answer:

The `-f` option is for `--force`.

بدون در خواست از کاربر فابل هارو حذف میکنه

### Example:

```bash
rm -f filename.txt
```
