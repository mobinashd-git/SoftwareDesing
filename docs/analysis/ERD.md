# Entity Relationship Diagram

## User

```text
id
fullName
phone
role
createdAt
```

توضیح:
- ولی و دانشجو از یک حساب استفاده می‌کنند.

---

## Student

```text
id
userId
gradeId
registrationDate
status
```

---

## Grade

```text
id
title
baseTuition
```

---

## ExtraClass

```text
id
title
tuition
capacity
active
```

---

## StudentExtraClass

```text
studentId
extraClassId
```

---

## TuitionItem

```text
id
title
amount
required
```

نمونه:
- کتاب
- آزمون
- هزینه ثبت نام

---

## Discount

```text
id
title
percent
condition
active
```

نمونه:
- اولین ثبت نام

---

## Enrollment

```text
id
studentId
totalAmount
discountAmount
finalAmount
createdAt
```

---

## Installment

```text
id
enrollmentId
number
amount
dueDate
status
```

status:
Pending
Paid
Overdue

---

## Payment

```text
id
installmentId
amount
gatewayRef
paymentDate
status
```

---

## FinancialRecord

```text
id
studentId
total
paid
remaining
```
