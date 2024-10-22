# 請模仿 MidtermReview-Sample.pdf 中的 Single/Multiple Answer Question 風格，

以 LEC6-CloudProgramming.pdf 的内容出 Single and Multiple Answer Question 各 20 題，不可重复，並給出答案和解釋，例如在哪一頁，為什麼這將是考試的重點，in English

# Answer (GPT-4 Omni):

以下是基於 _LEC6-CloudProgramming.pdf_ 的單選和多選題目，每類各 20 題，並提供答案和解釋。

## 單選題

1. **What function do users write their program in for the Cloud programming model?**

   - 答案: Map and Reduce functions
   - 解釋: 這些函數是 MapReduce 框架的基礎。
   - 頁碼: 25

2. **What does the master do in the master-worker model?**

   - 答案: Assigns map and reduce tasks to workers
   - 解釋: 這個角色對於任務分配和執行至關重要。
   - 頁碼: 25

3. **What is the output of each Map function?**

   - 答案: Intermediate key, value pairs
   - 解釋: 理解輸出格式對處理框架至關重要。
   - 頁碼: 25

4. **What function merges the local data of each map worker?**

   - 答案: Combine function
   - 解釋: 此函數在將數據發送到網絡之前減少通信成本。
   - 頁碼: 25

5. **Which policy applies for synchronization between map and reduce workers?**

   - 答案: A simple policy
   - 解釋: 同步策略對於確保協調的任務執行很重要。
   - 頁碼: 25

6. **What is the role of a partition function in MapReduce?**

   - 答案: To hash intermediate key-value pairs into partitions
   - 解釋: 保證相同鍵的所有鍵值對存儲在相同區域[1]。
   - 頁碼: 25

7. **What is a key advantage of using Spark over MapReduce?**

   - 答案: Faster data processing by keeping data in memory
   - 解釋: Spark 通過 RDD 在內存中保持數據，從而提高效率[1]。
   - 頁碼: 54

8. **What is a Resilient Distributed Dataset (RDD) in Spark?**

   - 答案: A read-only dataset that can be kept in memory
   - 解釋: RDD 是一種可靠的分佈式數據集，用於提高存儲效率[1]。
   - 頁碼: 54

9. **How does HDFS ensure fault tolerance?**

   - 答案: By replicating data across multiple datanodes
   - 解釋: HDFS 通過多重複製來確保數據的可靠性[1]。
   - 頁碼: 40

10. **What is the main function of a Namenode in HDFS?**

    - 答案: Manage metadata and file system namespace
    - 解釋: Namenode 負責管理文件系統的元數據和名稱空間[1]。
    - 頁碼: 40

11. **What does speculative execution address in MapReduce?**

    - 答案: Slow-performing tasks (stragglers)
    - 解釋: 通過重新安排緩慢的任務來提高性能[1]。
    - 頁碼: 32

12. **Which component handles task scheduling in Hadoop's MapReduce?**

    - 答案: JobTracker
    - 解釋: JobTracker 負責任務分配和監控[1]。
    - 頁碼: 45

13. **In Spark, what is the role of a Cluster Manager?**

    - 答案: To manage resources across the cluster
    - 解釋: 集群管理器負責資源分配和管理[1]。
    - 頁碼: 53

14. **What is the purpose of a DataNode in HDFS?**

    - 答案: Store and retrieve actual data blocks
    - 解釋: DataNode 實際執行數據存儲和檢索操作[1]。
    - 頁碼: 40

15. **How does Erasure Coding improve reliability in HDFS?**

    - 答案: By using mathematical coding techniques to create parity checks
    - 解釋: 通過生成校驗位來提高數據可靠性[1]。
    - 頁碼: 42

16. **What problem does MapReduce's partitioning function solve?**

    - 答案: Ensures all key-value pairs with identical keys are stored together
    - 解釋: 保證相同鍵的數據被正確分區以便於後續處理[1]。
    - 頁碼: 27

17. **In Spark, what mechanism helps recover lost RDDs?**

    - 答案: Lineage mechanism
    - 解釋: 通過 lineage 機制，可以從父 RDD 恢復丟失的 RDD[1]。
    - 頁碼: 54

18. **What is a key feature of Hadoop's architecture?**

    - 答案: Scalability and fault tolerance through distributed computing
    - 解釋: Hadoop 能夠擴展並通過分佈式計算提供容錯能力[1]。
    - 頁碼: 36

19. **Which component in Spark executes tasks on worker nodes?**

    - 答案: Executor
    - 解釋: Executor 是在工作節點上執行任務的進程[1]。
    - 頁碼: 53

20. **How does MapReduce handle large-scale data processing efficiently?**
    - 答案: By decomposing tasks into smaller parallel processes
    - 解釋: MapReduce 將大型任務分解為小型並行進程以提高效率[1]。
    - 頁碼：48

## 多選題

1. **Which of the following are characteristics of MapReduce?**
   Options:
   A. It uses a master-worker model  
   B. It only allows single-threaded map tasks  
   C. It generates intermediate key-value pairs  
   D. It supports computation partitioning

   正確答案：A, C, D

   解釋：這些特徵是有效利用 MapReduce 功能的核心。

   頁碼：25

2. **Which tasks are performed by workers in a MapReduce framework?**  
   Options:
   A. Reading input data  
   B. Aggregating results  
   C. Running Reduce functions  
   D. Writing final output to disk

   正確答案：A, C, D

   解釋：這些任務定義了 MapReduce 工作者的運作結構。

   頁碼：25

3. **Which advantages does Spark have over traditional MapReduce frameworks?**  
   Options:
   A. In-memory data processing  
   B. Better fault tolerance  
   C. Faster iterative processing  
   D. Simpler programming model

   正確答案：A, C

   解釋：Spark 通過內存處理和快速迭代處理提供了顯著優勢，但它並不一定比傳統的 MapReduce 更具容錯性或更簡單的編程模型[1]。

4. **Which components are part of Hadoop's ecosystem?**  
   Options:
   A. HDFS  
   B. YARN  
   C. Hive  
   D. Docker

   正確答案：A, B, C

5. **In which scenarios is Spark preferred over Hadoop's MapReduce?**

Options:
A. Real-time data processing  
B. Batch processing with high latency tolerance  
C. Iterative machine learning algorithms  
D. Ad-hoc queries with low latency requirements

正確答案：A, C, D

解釋：Spark 更適合需要低延遲和快速迭代處理的場景，而不是高延遲批處理[1]。

6. **What are the main components of an HDFS architecture?**

Options:
A. NameNode  
B. DataNode  
C. TaskTracker  
D. JobTracker

正確答案：A, B

解釋：NameNode 和 DataNode 是 HDFS 的核心組件，而 TaskTracker 和 JobTracker 屬於 MapReduce 架構的一部分[1]。

7. **Which features make RDDs efficient for big data processing in Spark?**

Options:
A. In-memory storage capability  
B. Fault-tolerance through lineage tracking  
C. Supports SQL queries natively  
D. Automatic partitioning

正確答案：A, B, D

解釋：RDDs 提供內存存儲、通過 lineage 跟踪實現容錯以及自動分區功能，使其在大數據處理中非常高效，但 SQL 查詢需要額外支持如 Spark SQL 才能原生支持[1]。

8. **Which strategies are used by Hadoop to ensure fault tolerance?**

Options:
A. Data replication across nodes  
B. Checkpointing intermediate results  
C. Speculative execution of slow tasks (stragglers)  
D. Real-time monitoring and alerting

正確答案：A, C

解釋：Hadoop 通過數據複製和對緩慢任務進行推測執行來實現容錯，而檢查點和實時監控通常不是其主要策略的一部分[1]。

9. **Which operations are typically performed during the shuffle phase in MapReduce?**

Options:
A. Sorting intermediate keys  
B. Merging intermediate values with same keys  
C. Reading input splits from disk  
D.Sending sorted data to reduce tasks

正確答案：A, B, D

解釋：shuffle 階段包括對中間鍵進行排序、合併具有相同鍵的中間值以及將排序後的數據發送到 reduce 任務中，而讀取輸入拆分通常發生在 map 階段之前[1]。

10 .**Which benefits does erasure coding provide over traditional replication in HDFS？**

Options：
A．Reduces storage overhead  
B．Improves read/write performance  
C．Enhances reliability through parity checks  
D．Simplifies metadata management

正確答案：A，C

解釋 ：通過使用校驗位來提高可靠性，同時減少存儲開銷 ，但可能會影響讀寫性能 ，並且不一定簡化元數據管理 [1].

11 .**In what ways can Spark achieve lower latency compared to traditional systems？**

Options：
A．Avoiding disk I/O by storing data in memory  
B．Using speculative execution for slow tasks  
C．Minimizing network communication through locality-aware scheduling  
D．Pre-compiling code for faster execution

正確答案：A，C

解釋 ：Spark 通過內存存儲和本地感知調度來降低延遲 ，而推測執行主要用於容錯 ，而不是降低延遲 [1].

12 .**Which challenges are addressed by using distributed file systems like HDFS？**

Options：
A．Handling large-scale datasets efficiently  
B．Ensuring high availability through redundancy  
C．Providing real-time analytics capabilities  
D．Facilitating seamless integration with cloud services

正確答案：A，B

解釋 ：HDFS 通過冗餘來提高可用性 ，並有效地處理大規模數據集 ，但需要其他工具才能提供實時分析或與雲服務集成 [1].

13 .**What mechanisms help prevent race conditions in parallel programs？**

Options：
A．Locking shared resources  
B．Implementing transaction logs  
C．Using atomic operations  
D．Applying version control systems

正確答案：A，C

解釋 ：鎖定共享資源和使用原子操作是防止並行程序中競爭條件的常見機制 ，而事務日誌和版本控制系統通常不適用於此 [1].

14 .**Which factors contribute to making Hadoop an economical choice for big data processing？**

Options：
A．Open-source nature  
B．Ability to run on commodity hardware  
C．Built-in support for machine learning algorithms  
D．Integration with various cloud platforms

正確答案：A，B

解釋 ：Hadoop 是開源的 ，可以在商用硬件上運行 ，這使其成為經濟實惠的大數據處理選擇 ，但機器學習算法和雲平台集成通常需要附加工具 [1].

15 .**In which scenarios would you choose to use YARN over traditional resource management systems？**

Options：
A．Managing resources across multiple clusters  
B．Supporting diverse workloads simultaneously  
C．Providing high-level APIs for application development  
D．Ensuring backward compatibility with legacy systems

正確答案：A，B

解釋 ：YARN 可以跨多個集群管理資源 ，並支持同時處理多樣化工作負載 ，但不一定提供高級 API 或向後兼容性 [1].

16 .**Which advantages do cloud-based solutions offer compared to on-premise deployments？**

Options：
A．Scalability on demand  
B．Lower upfront costs  
C．Greater control over hardware configurations  
D．Enhanced security measures

正確答案：A，B

解釋 ：雲端解決方案提供按需擴展能力和較低的前期成本 ，但硬件配置控制通常較少 ，安全措施也因供應商而異 [1].

17 .**How do containerization technologies like Docker enhance cloud computing environments？**

Options：
A．Enabling consistent deployment across platforms  
B．Reducing application startup times significantly  
C Supporting fine-grained access control policies  
D Simplifying dependency management

正確答案 ： A，D

解釋 ： Docker 等容器技術通過簡化依賴管理和跨平台一致部署來增強雲計算環境，但不一定顯著降低啟動時間或支持細粒度訪問控制策略 [2].

18 .**Which considerations should be taken into account when designing distributed applications for the cloud？**

Options：
A Network latency and bandwidth limitations  
B Fault tolerance and redundancy strategies  
C Licensing costs associated with proprietary software  
D Compliance requirements specific to industry regulations

正確答案 ： A，B

解釋 ： 設計雲端分布式應用時應考慮網絡延遲 、帶寬限制以及容錯策略等因素，而許可費用和合規要求則取決於具體情況 [2].

19 .**What benefits do serverless architectures provide over traditional server-based models？**

Options：
A Eliminating infrastructure management overhead  
B Allowing seamless scaling based on demand fluctuations  
C Offering built-in support for complex workflows  
D Enabling precise cost tracking per request

正確答案 ： A，B

解釋 ： 無服務架構消除了基礎設施管理負擔 ，允許根據需求波動無縫擴展，但複雜工作流支持通常需要額外配置 [2].

20 .**How can organizations leverage hybrid cloud strategies effectively？**

Options：
A Combining public and private clouds for optimal resource utilization  
B Ensuring seamless interoperability between different cloud providers  
C Centralizing all IT operations within a single platform  
D Implementing standardized security protocols across environments

正確答案 ： A，B

解釋 ： 混合雲策略通過結合公有雲與私有雲來優化資源利用率 ，並確保不同供應商之間無縫互操作性 ，而非集中所有 IT 操作或強制標準化安全協議 [2].

# Citations:

[1] [LEC6-CloudProgramming.pdf](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_73f844c9-478d-48c2-80b8-1b25d582a5ee/b03955f3-cc38-4823-ac4f-4a43a425f9a6/LEC6-CloudProgramming.pdf)  
[2] [MidtermReview-Sample.pdf](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_73f844c9-478d-48c2-80b8-1b25d582a5ee/0aee43cb-1fb0-4782-bfb9-724298fa9186/MidtermReview-Sample.pdf)
