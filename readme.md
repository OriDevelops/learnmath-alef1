# בית הספר למתמטיקה - אתר תרגול

אתר אינטראקטיבי בעברית לתרגול מתמטיקה: פרבולות, משוואות עם מכנים, גיאומטריה אנליטית והוכחות.

## איך להעלות את האתר לאינטרנט

### דרך 1: GitHub Pages (מומלץ - חינם וקבוע)

#### שלב 1: צור חשבון GitHub
היכנס ל-[github.com](https://github.com) ופתח חשבון אם אין לך.

#### שלב 2: צור repository חדש
1. לחץ על הפלוס בפינה הימנית העליונה ובחר "New repository"
2. תן שם, למשל: `learn-math`
3. השאר אותו "Public"
4. **אל תסמן** את "Add a README" - יש לנו כבר אחד
5. לחץ "Create repository"

#### שלב 3: דחוף את הקבצים
פתח טרמינל בתיקייה הזו (`learn-math-site`) והרץ:

```bash
git remote add origin https://github.com/YOUR_USERNAME/learn-math.git
git push -u origin main
```

החלף את `YOUR_USERNAME` בשם המשתמש שלך ב-GitHub.

> **הערה:** GitHub יבקש ממך להתחבר. אם זו הפעם הראשונה, צור [Personal Access Token](https://github.com/settings/tokens) (סוג: classic, הרשאה: repo) והשתמש בו כסיסמה.

#### שלב 4: הפעל את GitHub Pages
1. בעמוד ה-repository ב-GitHub, לחץ על "Settings" (הגדרות)
2. בתפריט השמאלי, לחץ על "Pages"
3. תחת "Source", בחר "Deploy from a branch"
4. תחת "Branch", בחר `main` ו-`/ (root)`
5. לחץ "Save"

#### שלב 5: גש לאתר
תוך כדקה האתר יהיה זמין בכתובת:
```
https://YOUR_USERNAME.github.io/learn-math/
```

---

### דרך 2: Netlify Drop (הכי מהיר, ללא Git)

הדרך הכי פשוטה ומהירה (חצי דקה):

1. גש ל-[https://app.netlify.com/drop](https://app.netlify.com/drop)
2. גרור את התיקייה `learn-math-site` (או רק את `index.html`) לחלון
3. תקבל מיד כתובת חינמית כמו `https://random-name.netlify.app`
4. אופציונלי: התחבר עם GitHub/Google כדי לשמור על האתר ולהוסיף דומיין מותאם

---

### דרך 3: Vercel (גם חינם, עם Git)

1. גש ל-[vercel.com](https://vercel.com) והתחבר עם GitHub
2. לחץ "Import Project" ובחר את ה-repo שיצרת
3. לחץ "Deploy" - זה הכל

---

## איך לעדכן את האתר אחרי שינויים

אחרי שערכת את `index.html` ורצונך להעלות עדכון:

```bash
git add index.html
git commit -m "Update site"
git push
```

האתר יתעדכן אוטומטית תוך דקה.

## תכנים באתר

- **פרבולות**: הזזה אנכית, אופקית ומשולבת, כיווץ ומתיחה, הצגה סטנדרטית
- **חיתוכים**: בין פרבולה וישר (7 נקודות מסומנות), בין שתי פרבולות
- **משוואות עם מכנים**: פתרון בשלבים עם בדיקת תחום הצבה
- **גיאומטריה אנליטית**: מקבילית וטרפז במערכת צירים
- **הוכחות**: בעיות מקבילית וטרפז עם רמזים מתקדמים
