---
layout: post
title: Algorithm
image: /img/2019-29-05/algorithm.jpg
---

## Analysis of Algorithms

- Why performance analysis?
  - Có nhiều điều quan trọng cần quan tâm của 1 hệ thống như: thân thiện với người dùng, mô-đun hóa, security, maintainability(khả năng bảo trì), ...Vậy vì sao phải quan tâm tới performance(hiệu năng)?
  - Câu trả lời thật đơn giản: chúng ta sẽ có tất cả nhưng điều trên nếu chúng ta có performance(hiệu năng), performance là giấy thông hành để chúng ta đi đến nhưng khả năng tiếp theo của your software, your system,..
  - Và Performance bằng khả năng scale hệ thống của bạn, nhưng nên nhớ ý tưởng chỉ thành hiện thực khi nó chạy được (runable), khi trong thời gian thực tập 1 software engineer đã nói với tôi rằng: "Đầu tiên là làm cho chương trình của em chạy được, sau đó mới tính đến chuyện cải thiện hiệu suất(performance) của chương trình", 
  - Túm cái váy -> performance là vấn đề sống còn của 1 hệ thống, 1 software, ...
- Cho 2 giải thuật cho 1 bài toán, làm cách nào xác định cái nào tốt hơn?
  - Một cách ngây thơm chúng ta implement 2 giải thuật và run 2 program trên cùng 1 môi trường xem giải thuật nào tốn ít thời gian hơn và kết luận. Nhưng kết luận thật khó khăn, đối với list input A giải thuật 1 có vẻ nhanh hơn, còn list input B thì giải thuật 2 lại nhanh hơn.
  - Một số trường hợp khác như thì thời gian chạy sẽ rối rắm giữa 2 giải thuật.
- Vậy có cách nào mô hình hóa được giải thuật được tốt hơn. Cùng tìm hiểu nào !

### Asymptotic Analysis

- Asymptotic Analysis là 1 big idea để giải quyết vấn đề phân tích tính hiệu quả của 1 giải thuật.
- Asymptotic Analysis, chúng ta đánh giá performance bằng cách bỏ qua các điều kiện hằng, giả định input có kích thước đạt trạng thái bảo hòa ( -> INF).


## Ref

- [Analysis of Algorithms](https://www.geeksforgeeks.org/fundamentals-of-algorithms/#AnalysisofAlgorithms)
