# Official test cases — expected vs prototype results

**Important:** These are local prototype simulations, not proof of official portal integration.

| ID | Synthetic input | Expected | Prototype actual | Status / difference |
|---|---|---|---|---|
| TC1 | Income ₹240,000; B.Tech; OBC | List matched schemes and save draft for top match | Local illustrative rules should match one or more schemes and create a local draft ID | PASS only for local demo logic; official scheme match is not verified |
| TC2 | Income = illustrative ceiling + ₹1 | Exclude with quoted rule | Local rule evaluator excludes above ceiling and shows demo rule | PASS only for local demo logic; source URL is placeholder |
| TC3 | Synthetic certificate over size limit | Compress copy, preserve original, upload, check readability | Size/hash behavior is simulated; no real compression/upload/readability check | FAIL / partial implementation, explicitly reported |
| TC4 | Draft DOB differs from student DOB | Block submission until corrected | Mismatch detection is demonstrated; no real submission portal exists | PASS for local validation demonstration only |

## Evidence capture
1. Open `index.html`.
2. Click **Run all 4 test cases**.
3. Capture a screenshot of the test table.
4. Click **Export evidence JSON** and preserve the downloaded file.
5. Save screenshots and JSON in the submission evidence folder.
