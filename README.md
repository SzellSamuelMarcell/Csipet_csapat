# Jane Street Real-Time Market Data Forecasting – 1. Mérföldkő

## Csapat adatok
**Csapat neve:** Csipet csapat  

**Csapattagok:**
- Hasas Tímea – `TZAS1B`
- Széll Sámuel Marcell – `BL046F`
- Sztancs László – `LDAG8S`

---

## Projektleírás
A projekt célja a Kaggle-ön meghirdetett **[Jane Street Real-Time Market Data Forecasting](https://www.kaggle.com/competitions/jane-street-real-time-market-data-forecasting)** verseny feladatának megoldása. 

A feladat során valós, éles kereskedési rendszerekből származó, anonimizált adathalmazzal dolgozunk. A cél egy olyan prediktív mélytanulási modell felépítése, amely képes megbízhatóan előrejelezni a különböző pénzügyi instrumentumok jövőbeli megtérülését leíró célváltozót, kiemelten a **`responder_6`** értéket.

---

## Futtatás
A mérföldkőhöz tartozó kód, adatelemzés (EDA), adat-előkészítés és a modell architektúrája az alábbi Jupyter Notebookban található:

- **Futtatandó fájl:** [`Csipet_csapat_1st_milestone.ipynb`](./Csipet_csapat_1st_milestone.ipynb)

### Főbb megvalósított lépések a notebookban
1. **Adatletöltés és -kezelés:** Parquet alapú hatékony adatbeolvasás.
2. **Feltáró adatelemzés (EDA):** Célváltozó (`responder_6`) statisztikai mutatói (volatilitás, ferdeség, csúcsosság, VaR), eloszlásvizsgálat és korrelációs analízis.
3. **Feature Engineering és Adat-előkészítés:** Időbeli (kronologikus) felbontás a look-ahead bias elkerülésére, robusztus skálázás és kategorikus változók kódolása.
4. **Modell architektúra:** Többágú Keras neurális hálózat entitás-beágyazással (Entity Embedding) és strukturált jellemzőkkel.
