PHÁT HIỆN HÀNH VI GIAN L ̣N TRONG KỲ THI TRỰC TUYẾN

Tác giả: Bùi Thế Tuấn, Lê Trần Xuân Dũng, 
Nguyễn Gia Hiền Minh

Khái quát: Ngày nay, việc chuyển hướng giáo dục truyền thống tại trường học sang trực tuyến dựa trên sự phát triển mạnh mẽ không ngừng nghỉ của mạng xã hội đang ngày một phổ biến hơn bao giờ hết. Ngoài những sự lợi ích mà nó mang lại thì song song với đó là những chở ngại trong việc kiểm soát tính khách quan trong quá trình thực hiện các bài kiểm tra. Vì vậy “Gian lận trong thi cử” đang dần trở thành một vấn đề đáng quan tâm hơn cả ở bất kì trình độ nào. Nghiên cứu này đề xuất một hệ thống thông minh có thể phát hiện gian lận trong thi cử dựa trên nhận diện khuôn mặt. Dựa vào việc yêu cầu phải sử dụng webcam trong toàn bộ quá trình thi, dựa vào việc phân tích ánh mắt và tư thế của đầu để theo dõi hành vi gian lận của thí sinh tham gia.

Từ khóa: online exam, cheating, classification, face detection, eye detection


 Mở đầu
I.1. Vấn đề
Các kỳ thi là một phần vô cùng quan trọng trong mọi chương trình giáo dục ở khắp các nơi trên thế giới. Trong bất cứ kỳ thi nào, việc xảy ra vấn đề gian lận thi cử đều có thể diễn ra. Theo khảo sát của Viện Khảo thí giáo dục Mỹ, tỷ lệ học sinh từng thực hiện hành vi gian lận trong thi cử hiện nay khoảng 75%, trong khi cách đây hơn nửa thế kỷ, con số này chỉ khoảng 20% [1]. Tình trạng gian lận trong thi cử không chỉ có ở học sinh kém mà lan sang cả học sinh có trình độ khá, thậm chí giỏi. Các em học sinh có xu hướng nghĩ rằng khi đi thi, các thí sinh khác cũng gian lận thì bản thân cũng nên gian lận để gia tăng điểm số, từ đó làm mất tính xác thực trong thi cử.
Khi các kỳ thi được thực hiện dưới hình thức offline trong một lớp học thông thường, các thí sinh sẽ bị giám thị trực tiếp giám sát trong quá trình diễn ra kỳ thi. Tuy nhiên, việc các giám thị giám sát trong cuộc thi trực tuyến lại vô cùng khó khăn. Nguy cơ xảy ra sai sót do sự giám sát từ xa trở thành mối lo ngại chính khi tổ chức một kỳ thi trực tuyến. Trong quá trình thi trực tuyến, giám thị có thể nhận thấy các hành vi có nguy cơ gian lận như cử động mắt bất thường hay ra khỏi màn hình giám sát. Tuy nhiên, họ cũng chỉ có thể giám sát thí sinh qua màn hình trực diện của mình trong khi thí sinh có thể tận dụng những góc chết của camera để tiến hành hành vi gian lận như sử dụng điện thoại di động để tra cứu, dùng ghi chú, giáo trình, hay thậm chí đeo tai nghe không dây và nhờ người khác nhắc đáp án từ xa.
		
I.2. Nghiên cứu liên quan
Trong [2],  một hệ thống giám sát trực tuyến mới được đề xuất sử dụng bộ dò khuôn mặt HOG và OpenCV thuật toán nhận dạng khuôn mặt. Nó được triển khai như một hệ thống phần mềm sử dụng FDDB và LFW bộ dữ liệu, do đó đạt được độ chính xác lên tới 97% khi nhận diện khuôn mặt và độ chính xác 99,3% cho khuôn mặt sự công nhận. Hệ thống này cũng có thể phát hiện các thiết bị như điện thoại di động trong bài kiểm tra trực tuyến.

Ở [3], một hệ thống thông minh đã được đề xuất để phát hiện các hoạt động gian lận của một học sinh đang cố gắng bài thi ở chế độ vật lý khi ở trong phòng thi thực. Với webcam được cài đặt thông minh các thiết bị đặt trên bàn học sinh, những hành vi đáng ngờ của họ  sẽ được theo dõi. Một thời gian thực video được ghi lại và sau đó được phân tích để xây dựng nền tảng kiến thức cho hệ thống. Hệ thống này có thể phát hiện ánh mắt và tư thế đầu của thí sinh để phát hiện gian lận. Từ đó có thể phân loại được hành vi nào đang gian lận

Một bài nghiên cứu chỉ ra rằng [4], các tác giả đã giới thiệu khái niệm gian lận trong thi tuyển trực tuyến và các phương pháp kiểm soát giống nhau. Các kỹ thuật đã được đề xuất để phát hiện và ngăn chặn học sinh gian lận.

Điều này được thực hiện thông qua xác thực liên tục bằng cách sử dụng giám sát trực tuyến. Người làm bài thi bị coi là gian lận hoặc không gian lận, bằng cách xem xét hai tham số dựa trên thời gian trên màn hình. Số lần thí sinh di chuyển ra khỏi màn hình, đo tổng thời gian cô ấy thực hiện điều này.

Nhận diện khuôn mặt được coi là bước đầu tiên được thực hiện trước khi quá trình nhận dạng có thể bắt đầu. Kỹ thuật nhận diện khuôn mặt được ra đời vào những năm 1970. Nó dần dần được cải thiện cùng với các công cụ hiện đại có thể được sử dụng trong thời gian thực. Điều này được nghiên cứu ở trong [5].

Ngoài ra ở bài nghiên cứu [6] [7], nhiều hệ thống đã được phát triển để phát hiện khuôn mặt mục tiêu ở những nơi có camera giám sát sử dụng phần mềm tốt nhất như MATLAB và Python để xử lý hình ảnh trong các hệ thống đó. Phần mềm này rất hiệu quả trong các hệ thống vân tay và nhiều hệ thống khác, chẳng hạn như hệ thống phân tích khớp mẫu được sử dụng để trích xuất tính năng, phân đoạn và tất cả các quá trình phát hiện và nhận dạng.

Một nghiên cứu với nội dung rất thú vị [8], khuôn khổ đề xuất cho việc giám sát bài thi trên máy tính dựa trên thiết bị điện tử thực hiện xác thực ứng viên bằng dấu vân tay của mình. Tiêu điểm định hướng mống mắt của học sinh được theo dõi. Một ngưỡng quy định được xem xét cho hệ thống. Nếu vượt quá mức góc nhìn hoặc mức độ giọng nói, người ta sẽ cho rằng ứng viên đang gian lận, rằng họ đang giao tiếp với ai đó. Việc triển khai được thực hiện bằng cách sử dụng ngôn ngữ Python, Java cho lập trình. Để giao tiếp với các tài nguyên, JDBC được sử dụng ở cấp cơ sở dữ liệu. MySQL cung cấp nền tảng để tạo và quản lý bài kiểm tra cùng với xác thực của cơ sở dữ liệu.

Như vậy, mặc dù đã có nhiều nỗ lực trong việc phát triển các hệ thống phát hiện gian lận trong bài thi trực tuyến, vẫn còn những khoảng trống và hạn chế cần được xem xét và giải quyết. Các nghiên cứu nên tập trung vào việc cải thiện độ chính xác và tính thực tế của các hệ thống, đồng thời xem xét việc ứng dụng chúng trong các tình huống thực tế để đảm bảo tính hiệu quả và hiệu suất.
I.3. Mục tiêu    
Tầm nhìn chính của chúng tôi là phát triển một hệ thống đáp ứng đầy đủ yêu cầu trong việc theo dõi hành vi gian lận trong thi trực tuyến, đặc biệt dựa trên các chỉ số từ ánh mắt và tư thế đầu. Chúng tôi đưa ra một giải pháp đơn giản nhưng mạnh mẽ để phát hiện và phân loại các hành vi gian lận trong bài thi trực tuyến. Hệ thống của chúng tôi sử dụng các mô hình và kỹ thuật để tự động thu thập hình ảnh thi cử mà không cần sự can thiệp của người giám sát. Các biện pháp xác minh khác như vân tay, giọng nói, cử động tay chân cũng có thể được tích hợp vào để cải thiện chất lượng của toàn bộ hệ thống bằng cách phát triển từ hệ thống ban đầu nhằm nâng cao chất lượng và độ tin cậy của hệ thống. Các biện pháp này không chỉ giúp tăng cường khả năng xác minh, mà còn giúp phát triển hệ thống từ một giai đoạn ban đầu đến một giải pháp toàn diện hơn.





 Khai thác dữ liệu
Trong quá trình tìm hiểu về chủ đề chống gian lận trong kỳ thi trực tuyến, việc tìm ra một bộ dữ liệu mở có thể đáp ứng yêu cầu của dự án là không thể. Vậy nên chúng tôi đã quyết định tự xây dựng và thu thập một bộ dữ liệu riêng biệt. 
Bằng cách thu thập hình ảnh thông qua việc sử dụng webcam trên thiết bị cá nhân. Với sự tham gia của ba cá nhân, quá trình ghi nhận được các trường hợp mô phỏng lại các trường hợp xảy ra trong quá trình thi cử của thí sinh như: nhìn thẳng, nhìn trái, nhìn phải, cúi đầu, liếc mắt, quay lưng, quay đầu, sử dụng tài liệu hay thiết bị điện tử được mô phỏng chính xác và chụp lại để phục vụ các bước xử lý hình ảnh tiếp theo (Hình 1). Kích thước hình ảnh các hình ảnh đã được thu thập là 640x480 pixel. Bộ dữ liệu sau đó được chia thành các tập dữ liệu test, train. Mỗi tập dữ liệu đều bao gồm các hình ảnh thể hiện hành vi gian lận và hành vi không gian lận. 





Hình 1. Một số mẫu thu thập
II.1. Tiền xử lý
Bộ dữ liệu ban đầu bao gồm khoảng gần 700 bức ảnh trong đó cả cả những hình ảnh bị lặp lại, bị mờ. Việc tiếp theo cần phải làm là loại bỏ những tấm ảnh mờ, không phù hợp trong việc dự đoán của mô hình. Sau đó là loại bỏ những hình ảnh trùng lặp khỏi bộ dữ liệu. Kết thúc quá trình này, bộ dữ liệu còn khoảng hơn 200 bức ảnh được lưu trữ lại để đưa vào việc huấn luyện mô hình về sau. 

Từ những hình ảnh sau khi được xử lý bước đầu, tiếp tục sử dụng mô hình DDN (Deep neural Network) để nhận dạng khuôn mặt. Khi đã nhận dạng được khuôn mặt, sử dụng Haar cascade để nhận dạng ánh mắt (Hình 2). Đây là những dữ liệu cuối cùng để đưa vào huấn luyện mô hình.




Hình 2. Ảnh sau quá trình tiền xử lý

II.2. Quá trình dán nhãn dữ liệu	
Quá trình chuẩn bị dữ liệu được thực hiện như sau: thí sinh sẽ làm bài thi trên máy tính, khi đó phần mềm thi sẽ chụp lại ngẫu nhiên các khoảnh khắc trong thời gian thi của thí sinh bằng webcam rồi chuyển các ảnh vào tập dữ liệu. Dữ liệu sau khi được tổng hợp  sẽ được xử lý bằng hai phương pháp: xác định khuôn mặt và xác định ánh mắt. 

Trong quá trình chuẩn bị, các ảnh mẫu về gian lận và không gian lận được đưa vào tập dữ liệu để dán nhãn cho từng ảnh. Sau khi dán nhãn, dữ liệu sẽ được chia vào các tập train, test và tiến hành huấn luyện mô hình. Kết thúc quá trình này tập dữ liệu bao gồm 2 nhãn : “cheating” và “not cheating” phục vụ cho quá trình huấn luyện và kiểm tra về sau. 
II.3. Các thành phần của bộ dữ liệu		

Bộ dữ liệu
Training
Test
Cheating
43
20
Not Cheating
56
34
Tổng
99
54









Bảng 1. Bảng thành phần bộ dữ liệu huấn luyện	

Đây là một bộ dữ liệu vừa phải, nhưng chúng ta vẫn có thể tiếp tục tăng số lượng thông qua quá trình augmentation để phục vụ nhu cầu huấn luyện và làm quen với dữ liệu lớn cho các sinh viên trong tương lai.	
Phương Pháp
Dự án này được thực hiện để phát hiện các hành vi gian lận thông qua khuôn mặt trong một buổi thi trực tuyến. Quy trình gồm hai giai đoạn: giai đoạn chuẩn bị và giai đoạn thi. 

Hình 3. Quá trình thực hiện

III.1. Nhận diện khuôn mặt

Có nhiều phương pháp đã được thử nghiệm để nhận diện khuôn mặt như YOLO v5, Haar Cascade và DNN. Trong số đó, phương pháp DNN được xem là phương pháp hiệu quả và tối ưu nhất trong việc nhận diện khuôn mặt.


DNN (Deep Neural Networks) là một loại mô hình máy học sâu mạnh mẽ, được huấn luyện trên dữ liệu lớn để nhận diện các đặc điểm và biểu hiện của khuôn mặt. Trong đó, mô hình ResNet-10 trong Caffe giúp nhận diện các đặc điểm phức tạp của khuôn mặt một cách chính xác.
Đầu tiên là xây dựng mô hình ResNet-10 bằng cách tạo tệp tin prototxt để lưu mô hình và tệp cấu hình đã tìm kiếm trước [12] [13]. Mô hình này đã sử dụng dữ liệu huấn luyện có sẵn và huấn luyện để cập nhật các trọng số, từ đó tạo ra các ma trận detections dựa trên các hình ảnh đầu vào.  
Để nhận diện khuôn mặt, một vòng lặp đã được tạo ra để lần lượt xử lý các phát hiện khuôn mặt từ ma trận detection, sau đó kiểm tra độ tin cậy sau phát hiện và vẽ viền khuôn mặt (chỉ tính khuôn mặt lớn nhất trên màn hình) nếu độ tin cậy lớn hơn 0.5. 
III.2. Xác định mắt
Dữ liệu đã được phát hiện và vẽ viền khuôn mặt sẽ tiếp tục được nhận diện mắt bằng Haar Cascade.

Haar Cascade là một phương pháp phổ biến được sử dụng để nhận diện các đối tượng trong hình ảnh và trong dự án này, mô hình đã được huấn luyện từ trước để phát hiện mắt [14]. Quá trình sử dụng bộ phân loại Haar Cascade sẽ tạo ra một danh sách các vùng chứa mắt được phát hiện, sau đó vẽ hình hộp xung quanh để làm nổi bật. 
III.3. Xử lý kết quả
Sau khi thu thập dữ liệu và nhận dạng mặt, mắt của thí sinh ở từng ảnh, hệ thống sẽ thực hiện phân loại dựa trên các tiêu chí về khuôn mặt như trên. Dữ liệu cần xử lý sẽ được đưa vào mô hình phát hiện gian lận đã được xây dựng, từ đó dự đoán hành vi gian lận hay không.

Phân Tích Kết Quả 
Trong phần này, các thử nghiệm đã được thiết kế để trả lời câu hỏi sau: Mô hình có thể phát hiện gian lận tốt đến mức nào, hiệu suất của toàn bộ mô hình như thế nào và ưu, nhược điểm của mô hình.

Đầu tiên là phân tích kết quả phân loại. Kết quả thu được từ quá trình giám sát và phân loại hành vi trong quá trình thi cử (Hình 3) đã cung cấp cái nhìn tổng quan về mức độ gian lận trong số tổng số ảnh thu được. Chúng tôi đã thu được tổng số 179 ảnh kết quả cụ thể chỉ có 11 ảnh được xác định là có dấu hiệu gian lận, trong khi 168 ảnh không có bất kỳ dấu hiệu nào của hành vi vi phạm quy tắc thi cử.



Hình 3. Kết quả phân loại

Sau đây là các biểu đồ để đánh giá mô hình. 




Biểu đồ 1. Đánh giá mô hình
Biểu đồ 1 biểu diễn các đánh giá về Accuracy, Precision, Recall, F1-score của mô hình với Accuracy đo lường tỷ lệ dự đoán chính xác trên tổng số mẫu, Precision đo lường tỷ lệ các dự án đúng (TP) trên tổng số các dự đoán dương (Positive prediction), Recall đo lường tỷ lệ các dự đoán đúng (TP) trên các mẫu thực sự dương (TP + FN) và F1-score là số trung hòa Recall và Prediction. Biểu đồ thể hiện rằng Accuracy của toàn bộ mô hình là 0,63%, Precision là 0,68%, Recall là 0,79% và F1-score là 0,73%.

Tuy đã phân loại được hình ảnh nhưng những con số này chưa phải là cao. Lý do là vì việc dự đoán đang được dựa trên mô hình đã được huấn luyện để phân tích khuôn mặt, chưa thực hiện được việc phát hiện các vật thể ngoài như điện thoại, sách vở trong hình ảnh phân loại. 


Biểu đồ 2. Độ chính xác                   Biểu đồ 3. Sự mất mát
Biểu đồ 2 thể hiện độ chính xác của mô hình với đường màu xanh là độ chính xác tập huấn luyện và màu vàng là độ chính xác tập kiểm tra. Độ chính xác trên tập huấn luyện cao hơn trên tập kiểm tra, điều này thể hiện rằng mô hình đang khớp với tập huấn luyện và chưa tổng quát tốt các dữ liệu mới.
Biểu đồ 3 thể hiện sự mất mát của mô hình với đường màu xanh là sự mất mát trên tập huấn luyện và đường màu vàng là sự mất mát trên tập kiểm tra. Giá trị sự mất mát trên tập kiểm tra cao hơn giá trị trên tập huấn luyện cho thấy rằng trong quá trình huấn luyện, mô hình đã bỏ sót thông tin và chưa dự đoán tốt các điểm dữ liệu mới. 

Kết Luận  
Sự phân tích chi tiết cho thấy rằng tỷ lệ hành vi gian lận chiếm một phần rất nhỏ trong số lượng tổng thể. Các hành vi gian lận thường liên quan đến việc rời mắt khỏi màn hình thường xuyên, thay đổi góc lấy nét không đồng nhất hoặc hành vi không tuân theo quy tắc thi cử. Trong khi đó, hầu hết số ảnh còn lại đều tuân thủ quy tắc và không có bất kỳ biểu hiện nghi ngờ nào.

Tuy nhiên, với số lượng lớn ảnh không có dấu hiệu gian lận, việc sử dụng các phương pháp giám sát và phân loại có thể hữu ích trong việc duy trì tính minh bạch và công bằng trong quá trình thi cử.

Việc cải thiện và tối ưu hóa hệ thống giám sát là điều cần thiết để nâng cao khả năng phát hiện và ngăn chặn hành vi gian lận một cách hiệu quả hơn trong tương lai.
Tham Khảo
	
[1] Princeton, N.J. – Sept. 8, 1999: Educational Testing Service and The Advertising Council today announced the launch of a national public service advertising campaign intended to discourage academic cheating.

[2] Istiak Ahmad, Fahad AlQurashi, Ehab Abozinadah and Rashid Mehmood, “A Novel Deep Learning-based Online Proctoring System using Face Recognition, Eye Blinking, and Object Detection Techniques” International Journal of Advanced Computer Science and Applications(IJACSA), 12(10), 2021. http://dx.doi.org/10.14569/IJACSA.2021.0121094

[3] P. Subbarayudu, B. S. Mohan, G. P. Kumar and D. S. John Deva Prasanna, "Detection of Anomalous Behaviour of a Student in Examination Hall Using Deep Learning Techniques," 2022 IEEE 2nd International Conference on Mobile Networks and Wireless Communications (ICMNWC), Tumkur, Karnataka, India, 2022, pp. 1-6, doi: 10.1109/ICMNWC56175.2022.10031695.

[4] Razan Bawarith, Dr. Abdullah Basuhail, Dr. Anas Fattouh and Prof. Dr. Shehab Gamalel-Din, “E-exam Cheating Detection System” International Journal of Advanced Computer Science and Applications(IJACSA), 8(4), 2017. http://dx.doi.org/10.14569/IJACSA.2017.080425

[5] Erik Hjelmås, Boon Kee Low, Face Detection: A Survey, Computer Vision and Image Understanding, Volume 83, Issue 3, 2001, Pages 236-274, ISSN 1077-3142

[6] H. Li, Z. Lin, X. Shen, J. Brandt and G. Hua, "A convolutional neural network cascade for face detection," 2015 IEEE Conference on Computer Vision and Pattern Recognition (CVPR), Boston, MA, USA, 2015, pp. 5325-5334, doi: 10.1109/CVPR.2015.7299170.

[7] Xiangyu Zhu, Z. Lei, Junjie Yan, D. Yi and S. Z. Li, "High-fidelity Pose and Expression Normalization for face recognition in the wild," 2015 IEEE Conference on Computer Vision and Pattern Recognition (CVPR), Boston, MA, USA, 2015, pp. 787-796, doi: 10.1109/CVPR.2015.7298679.

[8] G. B. Iwasokun, O. C. Akinyokun and T. G. Omomule, "Design of E-Invigilation Framework Using Multi-Modal Biometrics," 2019 15th International Conference on Electronics, Computer and Computation (ICECCO), Abuja, Nigeria, 2019, pp. 1-6, doi: 10.1109/ICECCO48375.2019.9043223.

[9] Ozdamli, F.; Aljarrah, A.; Karagozlu, D.; Ababneh, M. Facial Recognition System to Detect Student Emotions and Cheating in Distance Learning. Sustainability 2022, 14, 13230. https://doi.org/10.3390/su142013230

[10] Masud, M.M., Hayawi, K., Mathew, S.S., Michael, T., El Barachi, M. (2022). Smart Online Exam Proctoring Assist for Cheating Detection. In: Li, B., et al. Advanced Data Mining and Applications. ADMA 2022. Lecture Notes in Computer Science(), vol 13087. Springer, Cham. https://doi.org/10.1007/978-3-030-95405-5_9

[11] Coghlan, S., Miller, T. & Paterson, J. Good Proctor or “Big Brother”? Ethics of Online Exam Supervision Technologies. Philos. Technol. 34, 1581–1606 (2021). https://doi.org/10.1007/s13347-021-00476-1

[12] Dnn_samples_face_detector/res10_300x300_ssd_iter_140000.caffemodel

[13] Dnn/face_detector/deploy.prototxt

[14]HaarCascade_eye.xml

