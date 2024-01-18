> Certain commercial entities, equipment, or materials may be identified in this document in order to describe an experimental procedure or concept adequately. Such identification is not intended to imply recommendation or endorsement by the National Institute of Standards and Technology (NIST), nor is it intended to imply that the entities, materials, or equipment are necessarily the best available for the purpose.

本書では、実験手順や概念を適切に説明するために、特定の商業団体、装置、または材料が特定される場合がある。このような特定は、米国国立標準技術研究所（NIST）による推奨や推薦を意味するものではなく、また、その事業体、材料、装置が必ずしもその目的に対して利用可能な最良のものであることを意味するものでもない。

> There may be references in this publication to other publications currently under development by NIST in accordance with its assigned statutory responsibilities. The information in this publication, including concepts and methodologies, may be used by federal agencies even before the completion of such companion publications. Thus, until each publication is completed, current requirements, guidelines, and procedures, where they exist, remain operative. For planning and transition purposes, federal agencies may wish to closely follow the development of these new publications by NIST.

本書には、NISTがその法定責任に基づき現在開発中の他の出版物への参照が含まれている場合がある。概念や方法論を含む本書の情報は、そのような関連出版物の完成前であっても、連邦機関によって使用される可能性がある。従って、各出版物が完成するまでは、現行の要求事項、ガイドライン、手順が存在する場合は、それらが引き続き有効である。計画及び移行の目的で、連邦機関はNISTによるこれらの新出版物の開発を注意深く見守ることが望ましい。

>Organizations are encouraged to review all draft publications during public comment periods and provide feedback to NIST. Many NIST cybersecurity publications, other than the ones noted above, are available at

各機関は、パブリックコメント期間中にすべての出版物の草案を検討し、NIST にフィードバックを提供することが推奨される。上記以外の多くの NIST サイバーセキュリティ関連出版物は、以下で入手可能である。

https://csrc.nist.gov/publications

# Authority / 権威
> This publication has been developed by NIST in accordance with its statutory responsibilities under the Federal Information Security Modernization Act (FISMA) of 2014, 44 U.S.C. § 3551 et seq., Public Law (P.L.) 113-283.

本書は、Federal Information Security Modernization Act (FISMA) of 2014, 44 U.S.C. § 3551 et seq.、Public Law (P.L.) 113-283 に基づく法的責任に基づき、NISTが作成したものである。

> NIST is responsible for developing information security standards and guidelines, including minimum requirements for federal information systems, but such standards and guidelines shall not apply to national security systems without the express approval of appropriate federal officials exercising policy authority over such systems. This guideline is consistent with the requirements of the Office of Management and Budget (OMB) Circular A-130.

NISTは、連邦情報システムに対する最低要件を含む情報セキュリティ基準およびガイドラインを策定する責任を負うが、そのような基準およびガイドラインは、そのようなシステムに対する政策権限を行使する適切な連邦政府当局者の明示的な承認がない限り、国家安全保障システムに適用してはならない。本ガイドラインは、Office of Management and Budget (OMB) Circular A-130 の要件と一致している。

> Nothing in this publication should be taken to contradict the standards and guidelines made mandatory and binding on federal agencies by the Secretary of Commerce under statutory authority. Nor should these guidelines be interpreted as altering or superseding the existing authorities of the Secretary of Commerce, Director of the OMB, or any other federal official. This publication may be used by nongovernmental organizations on a voluntary basis and is not subject to copyright in the United States. Attribution would, however, be appreciated by NIST.

本書のいかなる内容も、法的権限に基づき商務長官が連邦政府機関に義務付け、拘束力を持たせた基準やガイドラインと矛盾するものであってはならない。また、本ガイドラインは、商務長官、OMB長官、その他の連邦政府当局者の既存の権限を変更したり、これに取って代わるものと解釈されるべきでもない。本書は、非政府組織が任意で使用することができ、米国における著作権の対象ではない。ただし、NISTは帰属を認める。

# NIST Technical Series Policies / NISTテクニカルシリーズ方針
* [Copyright, Fair Use, and Licensing Statements](https://doi.org/10.6028/NIST-TECHPUBS.CROSSMARK-POLICY)
* [NIST Technical Series Publication Identifier Syntax](https://www.nist.gov/document/publication-identifier-syntax-nist-technical-series-publications)

# Publication History
* Approved by the NIST Editorial Review Board on 2022-11-08
* Supersedes NIST SP 800-160 Vol. 1 (Nov. 2016; updated 2018-03-21)

https://doi.org/10.6028/NIST.SP.800-160v1

# How to Cite this NIST Technical Series Publication:
Ross R, McEvilley M, Winstead M (2022) Engineering Trustworthy Secure Systems. (National Institute of Standards and Technology, Gaithersburg, MD), NIST Special Publication (SP) NIST SP 800-160v1r1.

https://doi.org/10.6028/NIST.SP.800-160v1r1

# Author ORCID iDs
Ron Ross: 0000-0002-1099-9757

# Contact Information
* security-engineering@nist.gov
* National Institute of Standards and Technology
* Attn: Computer Security Division, Information Technology Laboratory
* 100 Bureau Drive (Mail Stop 8930) Gaithersburg, MD 20899-8930

**All comments are subject to release under the Freedom of Information Act (FOIA).**

# Abstract / 要旨

> This publication describes a basis for establishing principles, concepts, activities, and tasks for engineering trustworthy secure systems. Such principles, concepts, activities, and tasks can be effectively applied within systems engineering efforts to foster a common mindset to deliver security for any system, regardless of the system’s purpose, type, scope, size, complexity, or the stage of its system life cycle. The intent of this publication is to advance systems engineering in developing trustworthy systems for contested operational environments (generally referred to as systems security engineering) and to serve as a basis for developing educational and training programs, professional certifications, and other assessment criteria.

本書は、信頼できるセキュアなシステムを設計するための原則、概念、活動、タスクを確立するための基礎について記述している。このような原則、概念、活動、及びタスクは、システムの目的、種類、範囲、規模、複雑さ、又はシステムライフサイクルの段階に関係なく、あらゆるシステムのセキュリティを実現するための共通の考え方を醸成するために、システム工学の取り組みの中で効果的に適用することができる。本書の目的は、競合する運用環境に対して信頼できるシステムを開発するシステム工学（一般にシステムセキュリティ工学と呼ばれる）を発展させ、教育・訓練プログラム、専門家認定、その他の評価基準を開発するための基礎とすることである。

# Keywords / キーワード
> assurance; developmental engineering; engineering trades; field engineering; implementation; information security; information security policy; inspection; integration; penetration testing; protection needs; requirements analysis; resilience; review; risk assessment; risk management; risk treatment; security architecture; security design; security requirements; specifications; stakeholders; system of systems; system component; system element; system life cycle; systems; systems engineering; systems security engineering; trustworthiness; validation; verification

保証;開発エンジニアリング;エンジニアリング業務;フィールドエンジニアリング;実装; 情報セキュリティ; 情報セキュリティ方針; 検査; 統合; 侵入テスト; 保護ニーズ; 要求分析; 回復力; レビュー; リスク評価; リスク管理; リスク処理; セキュリティ・アーキテクチャ; セキュリティ設計; セキュリティ要件; 仕様; 利害関係者; システム・オブ・システム; システム・コンポーネント; システム要素; システム・ライフサイクル; システム; システムエンジニアリング; システムセキュリティエンジニアリング; 信頼性; 妥当性確認; 検証

# Reports on Computer Systems Technology / コンピュータ システム技術に関するレポート
> The Information Technology Laboratory (ITL) at the National Institute of Standards and Technology (NIST) promotes the U.S. economy and public welfare by providing technical leadership for the Nation’s measurement and standards infrastructure. ITL develops tests, test methods, reference data, proof of concept implementations, and technical analyses to advance the development and productive use of information technology. ITL’s responsibilities include the development of management, administrative, technical, and physical standards and guidelines for the cost-effective security and privacy of other than national security-related information in federal information systems. The Special Publication 800-series reports on ITL’s research, guidelines, and outreach efforts in information system security, and its collaborative activities with industry, government, and academic organizations.

国立標準技術研究所（NIST）の情報技術研究所（ITL）は、国家の測定および標準インフラストラクチャのための技術的リーダーシップを提供することにより、米国経済と公共の福祉を促進する。ITLは、試験、試験方法、参照データ、概念実証実装、技術分析を開発し、情報技術の開発と生産的利用を促進している。ITLの責任には、連邦情報システムにおける国家安全保障関連情報以外のコスト効率の良いセキュリティとプライバシーのための管理、管理、技術、物理的な標準とガイドラインの開発が含まれる。Special Publication 800シリーズは、情報システム・セキュリティに関するITLの研究、ガイドライン、アウトリーチ活動、および産業界、政府機関、学術機関との協力活動について報告している。

# Patent Disclosure Notice / 特許開示通知

> NOTICE: ITL has requested that holders of patent claims whose use may be required for compliance with the guidance or requirements of this publication disclose such patent claims to ITL. However, holders of patents are not obligated to respond to ITL calls for patents and ITL has not undertaken a patent search in order to identify which, if any, patents may apply to this publication.

注意：ITLは、本書のガイダンスまたは要件に準拠するために使用が必要となる特許請求の範囲の保有者に対し、当該特許請求の範囲をITLに開示するよう要請している。ただし、特許権者はITLの特許募集に応じる義務はなく、ITLは、本書に該当する特許があるとしても、それを特定するための特許調査を行っていない。

> As of the date of publication and following call(s) for the identification of patent claims whose use may be required for compliance with the guidance or requirements of this publication, no such patent claims have been identified to ITL.

本書の発行日および、本書のガイダンスまたは要件に準拠するために使用が必要とされる可能性のある特許請求の範囲の特定を求めた後の時点で、そのような特許請求の範囲はITLに特定されていない。

No representation is made or implied by ITL that licenses are not required to avoid patent infringement in the use of this publication.

ITLは、本書の使用において特許侵害を回避するためのライセンスが不要であることを表明するものではなく、また示唆するものでもない。

# Disclaimer / 免責事項
> This publication should be used as a supplement to International Standard ISO/IEC/IEEE 15288 and other supporting international standards. It is recommended that organizations using this publication obtain the appropriate international standards to understand the context of the material in Appendices G through K. Content from ISO/IEC/IEEE 15288 referenced in this publication is used with permission from the Institute of Electrical and Electronics Engineers. It is noted as follows:

本書は、国際規格ISO/IEC/IEEE 15288及びその他の国際規格の補足として使用される。本書で参照されているISO/IEC/IEEE 15288の内容は、米国電気電子学会（Institute of Electrical and Electronics Engineers）の許可を得て使用している。以下のように記されている：

> * Reprinted with permission from IEEE, Copyright IEEE 2015, All rights reserved.

* IEEE, Copyright IEEE 2015, All rights reservedより許可を得て転載。

> The reprinted material has been updated to reflect any changes in the international standard.

再版された資料は、国際規格の変更を反映して更新されている。

# Table of Contents / 目次
* [Introduction / はじめに](Introduction.md)
  * [Purpose and Applicability / 目的と適用範囲](Introduction.md#Purpose-and-Applicability--目的と適用範囲)
  * [Target Audience / 対象読者](Introduction.md#Target-Audience--対象読者)
  * [How to Use this Publication / 本書の使い方](Introduction.md#How-to-Use-this-Publication--本書の使い方)
  * [Organization of this Publication / 本書の構成](Introduction.md#Organization-of-this-Publication--本書の構成)
* [Systems Engineering Overview / システムエンジニアリングの概要](Systems_Engineering_Overview.md)
  * [System Concepts / システムの概念](Systems_Engineering_Overview.md#System-Concepts--システムの概念)
    * Systems and System Structure / システムとシステム構造
    * Interfacing, Enabling, and Interoperating Systems / インターフェイス化、有効化、およびシステム間相互運用
  * [Systems Engineering Foundations / システムエンジニアリングの基礎](Systems_Engineering_Overview.md#Systems-Engineering-Foundations--システムエンジニアリングの基礎)
  * [Trust and Trustworthiness / 信用と信用度](Systems_Engineering_Overview.md#Trust-and-Trustworthiness--信用と信用度)
* [System Security Concepts / システムセキュリティの概念](System_Security_Concepts.md)
  * The Concept of Security / セキュリティの概念
  * The Concept of an Adequately Secure System / 十分に安全なシステムの概念
  * Characteristics of Systems / システムの特徴
  * The Concept of Assets / 資産の概念
  * The Concepts of Loss and Loss Control / 損失と損失コントロールの概念
  * Reasoning about Asset Loss / 資産損失についての推論
  * Determining Protection Needs / 保護ニーズの特定
  * System Security Viewpoints / システムセキュリティの観点
  * Demonstrating System Security / システムセキュリティの実証
  * Systems Security Engineering / システムセキュリティエンジニアリング
* [Systems Security Engineering Framework / システムセキュリティエンジニアリングの枠組み](Systems_Security_Engineering_Framework.md)
  * The Problem Context / 問題の文脈
  * The Solution Context / 解決策の文脈
  * The Trustworthiness Context / 信用度 の文脈

* References 
* Appendix A. [Acronyms / アクロニム](Acronyms.md)
* Appendix B. [Glossary / 用語集](Glossary.md)
* Appendix C. [Security Policy and Requirements / セキュリティポリシーと要件](Security_Policy_and_Requirements.md)
* C.1. Security Policy / セキュリティポリシー
* C.2. Security Requirements / セキュリティ要件
* C.3. Distinguishing Requirements, Policy, and Mechanisms / 要件、ポリシー、メカニズムの区別
* Appendix D. [Trustworthy Secure Design / 信用度の高いセキュアな設計](Trustworthy_Secure_Design.md)
* D.1. Design Approach for Trustworthy Systems / 信用度の高いシステムのための設計アプローチ
* D.2. Design Considering Emergence / 創発を考慮した設計
* D.3. Security Design Order of Precedence / セキュリティ設計の優先順位
* D.4. Functional Design Considerations / 機能設計の考慮事項
* Appendix E. [Principles for Trustworthy Secure Design / 信用度の高いセキュアな設計のための原則](Principles_for_Trustworthy_Secure_Design.md)
* E.1. Anomaly Detection / アノマリ検知
* E.2. Clear Abstractions / 明確な抽象化
* E.3. Commensurate Protection / 相応の保護
* E.4. Commensurate Response / 相応の対応 (response)
* E.5. Commensurate Rigor / 相応の厳格さ (rigor)
* E.6. Commensurate Trustworthiness / 相応の信頼性 (trustworthness)
* E.7. Compositional Trustworthiness / 合成的な信頼性 (trustworthness)
* E.8. Continuous Protection / 継続的な保護
* E.9. Defense In Depth / 多重防護
* E.10. Distributed Privilege / 分散された特権
* E.11. Diversity (Dynamicity) / 多様性（動的性）
* E.12. Domain Separation / ドメイン分離
* E.13. Hierarchical Protection / 階層的な保護
* E.14. Least Functionality / 最小の機能
* E.15. Least Persistence / 最小の持続性
* E.16. Least Privilege / 最小の特権
* E.17. Least Sharing / 最小の共有
* E.18. Loss Margins / 損失マージン
* E.19. Mediated Access / 仲介されたアクセス
* E.20. Minimal Trusted Elements / 信頼される要素の最小化
* E.21. Minimize Detectability / 検出可能性の最小化
* E.22. Protective Defaults / 保護的なデフォルト
* E.23. Protective Failure / 保護的な失敗
* E.24. Protective Recovery / 保護的なリカバリ
* E.25. Reduced Complexity / 複雑さの軽減
* E.26. Redundancy / 冗長性
* E.27. Self-Reliant Trustworthiness / 自立した信用度
* E.28. Structured Decomposition and Composition / 構造化された分解と合成
* E.29. Substantiated Trustworthiness / 実証された信用度
* E.30. Trustworthy System Control / 信用度の高いシステム コントロール
* Appendix F. [Trustworthiness and Assurance / 信用度と保証](Trustworthiness_and_Assurance.md)
* F.1. Trust and Trustworthiness / 信用と信用度
* F.2. Assurance / 保証
* Appendix G. [System Life Cycle Processes Overview / システムライフサイクルプロセスの概要](System_Life_Cycle_Processes_Overview.md)
* G.1. Process Overview / プロセスの概要
* G.2. Process Relationships / プロセスの関係
* Appendix H. [Technical Processes / 技術的プロセス](Technical_Processes.md)
* H.1. Business or Mission Analysis / ビジネスまたはミッションの分析
* H.2. Stakeholder Needs and Requirements Definition / 利害関係者のニーズと要件の定義
* H.3. System Requirements Definition / システム要件の定義
* H.4. System Architecture Definition / システムアーキテクチャの定義
* H.5. Design Definition / デザインの定義
* H.6. System Analysis / システム分析
* H.7. Implementation / 実装
* H.8. Integration / 統合 (インテグレーション)
* H.9. Verification / 検証
* H.10. Transition / 遷移
* H.11. Validation / バリデーション
* H.12. Operation / 運用
* H.13. Maintenance / メンテナンス
* H.14. Disposal / 廃棄
* Appendix I. [Technical Management Processes / 技術的マネジメントプロセス](Technical_Management_Processes.md)
* I.1. Project Planning / プロジェクトの計画
* I.2. Project Assessment and Control / プロジェクトのアセスメントとコントロール
* I.3. Decision Management / 意思決定マネジメント
* I.4. Risk Management / リスク マネジメント
* I.5. Configuration Management / 構成設定マネジメント
* I.6. Information Management / 情報マネジメント
* I.7. Measurement / 測定
* I.8. Quality Assurance / 品質保証
* Appendix J. [Organizational Project-Enabling Processes / 組織的なプロジェクト実現プロセス](Organizational_Project_Enabling_Processes.md)
* J.1. Life Cycle Model Management / ライフサイクルモデル マネジメント
* J.2. Infrastructure Management / インフラストラクチャ マネジメント
* J.3. Portfolio Management / ポートフォリオ マネジメント
* J.4. Human Resource Management / 人的リソース マネジメント
* J.5. Quality Management / 品質マネジメント
* J.6. Knowledge Management / 知識マネジメント
* Appendix K. [Agreement Processes / 契約プロセス](Agreement_Processes.md)
* K.1. Acquisition / 取得
* K.2. Supply / 供給
* Appendix L. Change Log / 更新履歴

## List of Tables
* Table 1. Common Asset Classes 
* Table 2. Loss Control Objectives
* Table 3. Essential Design Criteria for Mechanisms
* Table 4. Principles for Trustworthy Secure Design 
* Table 5. System Life Cycle Processes 
* Table 6. Change Log 

## List of Figures
* Fig. 1. Basic System and System Element Relationship
* Fig. 2. Model for a System and its Elements 
* Fig. 3. System of Interest and Interfacing Systems 
* Fig. 4. System Security and Cost/Schedule/Technical Performance 
* Fig. 5. Idealized Notional Secure System State Transitions
* Fig. 6. Reasoning about Asset Protection 
* Fig. 7. Defining Protection Needs
* Fig. 8. Relationship among Asset, Loss, and Consequence 
* Fig. 9. Systems Engineering and Other Specialty Engineering Disciplines
* Fig. 10. Systems Security Engineering Framework
* Fig. 11. Allocation of Security Policy Responsibilities 
* Fig. 12. Stakeholder and System Requirements 
* Fig. 13. Entities that Affect Security Requirements Development 
* Fig. 14. Relationship between Mechanisms and Security Policy Enforcement 
* Fig. 15. Design Approach in a Systems Security Engineering Framework 
* Fig. 16. Balanced Design Strategy for Achieving Trustworthy Secure Systems 
* Fig. 17. Assurance and Degree of Rigor in Realizing a Capability Need 
* Fig. 18. Types of Personnel and Roles that Support Life Cycle Processes 
* Fig. 19. Relationships Among Life Cycle Processes 

# Preface / 序文
> On May 12, 2021, the President signed an Executive Order (EO) on Improving the Nation's Cybersecurity [1]. The Executive Order stated, The United States faces persistent and increasingly sophisticated malicious cyber campaigns that threaten the public sector, the private sector, and ultimately the American people’s security and privacy. The Federal Government must improve its efforts to identify, deter, protect against, detect, and respond to these actions and actors.

2021年5月12日、大統領は国家のサイバーセキュリティを向上させることに関する大統領令（EO）に署名した。この大統領令には、以下のように記されている。「アメリカ合衆国は、公共部門、民間部門、そして究極的にはアメリカ国民の安全とプライバシーを脅かす、執拗でますます巧妙な悪意のあるサイバーキャンペーンに直面している。連邦政府は、これらの行動と行為者を特定し、抑止し、防御し、検出し、対応するための努力を強化しなければならない。」

> The Executive Order further described the holistic nature of the cybersecurity challenges confronting the Nation with computing technology embedded in every type of system from general-purpose computing systems that support businesses to cyber-physical systems that control the operations in power plants and provide electricity to the American people. The Federal Government must bring the full scope of its authorities and resources to bear in order to protect and secure its computer systems, whether the systems are cloud-based, on-premises, or hybrid. The scope of protection and security must include systems that process data (i.e., information technology [IT]) and systems that run the machinery that ensure our safety (i.e., operational technology [OT]).

大統領令はさらに、国が直面しているサイバーセキュリティの課題の全体的な性質を詳述している。「コンピューティング技術は、ビジネスをサポートする汎用コンピューティングシステムから、発電所の運営を制御しアメリカ国民に電力を提供するサイバー物理システムに至るまで、あらゆる種類のシステムに組み込まれている。連邦政府は、その権限と資源の全範囲を活用して、コンピュータシステムを保護しセキュリティを確保しなければならない。これらのシステムがクラウドベースであれ、オンプレミスであれ、ハイブリッドであれ、保護とセキュリティの範囲は、データを処理するシステム（すなわち情報技術[IT]）と、私たちの安全を保証する機械を稼働させるシステム（すなわち運用技術[OT]）を含まなければならない。」

> In response to the EO, there is a need to:

大統領令に応じて、以下のような対応が必要である：

> * Identify stakeholder assets and protection needs

* 利害関係者の資産と保護ニーズを特定する。

> * Provide protection commensurate with the significance of asset loss and correlated with threat and adversary capabilities

* 資産損失の重要性に見合った保護を提供し、脅威と敵対者の能力に応じてそれを調整する。

> * Develop scenarios and model the complexity of systems to provide a rigorous basis to reason about, manage, and address the uncertainty associated with that complexity

* システムの複雑さをモデル化しシナリオを開発し、その複雑さに伴う不確実性を理解し、管理し、対処するための厳格な基盤を提供する。

> * Adopt an engineering-based approach that addresses the principles of trustworthy secure design and apply those principles throughout the system life cycle

* 信用度のある安全な設計の原則に対応する工学ベースのアプローチを採用し、システムのライフサイクル全体にわたって信頼性の原則を適用する。

> Building trustworthy, secure systems cannot occur in a vacuum with stovepipes for software, hardware, information technology, and the human element (e.g., designers, operators, users, attackers of these systems). Rather, it requires a transdisciplinary approach to protection, a determination across all assets where loss could occur, and an understanding of adversity, including how adversaries attack and compromise systems. As such, this publication addresses considerations for the engineering-driven actions necessary to develop defensible and survivable systems, including the components that compose and the services that depend on those systems. The objective is to address security issues from the perspective of stakeholder requirements and protection needs and to use established engineering processes to ensure that such requirements and needs are addressed with appropriate fidelity and rigor across the entire life cycle of the system.

信用度が高く、安全なシステムの構築は、ソフトウェア、ハードウェア、情報技術、そして人間要素（例えば、これらのシステムの設計者、運用者、ユーザー、攻撃者）のための孤立した領域で行われることはない。むしろ、それは保護に関して学際的なアプローチを要求し、損失が発生しうるすべての資産にわたる決意と、敵意を含む逆境への理解、特に敵がシステムを攻撃し妥協させる方法を理解することを必要とする。したがって、本書は、システムを構成するコンポーネントやそれらのシステムに依存するサービスを含む、防御可能で生存可能なシステムを開発するために必要な工学駆動の行動に関する考慮事項に対処する。目的は、利害関係者の要件と保護ニーズの観点からセキュリティ問題に対処し、確立された工学プロセスを使用して、そのような要件とニーズがシステムの全ライフサイクルにわたって適切な忠実度と厳格さで対処されるようにすることである。

> Engineering trustworthy, secure systems is a significant undertaking that requires a substantial investment in the requirements, architecture, and design of systems, components, applications, and networks. A trustworthy system provides compelling evidence to support claims that it meets its requirements to deliver the protection and performance needed by stakeholders. Introducing a disciplined, structured, and standards-based set of systems security engineering activities and tasks provides an important starting point and forcing function to initiate needed change.

信用度が高く、安全なシステムを工学的に構築することは、システム、コンポーネント、アプリケーション、ネットワークの要件、アーキテクチャ、設計への相当な投資を必要とする重要な取り組みである。信用度の高いシステムは、利害関係者に必要とされる保護と性能を提供するための要件を満たしているという主張を支持する説得力のある証拠を提供する。規律ある、構造化された、標準に基づく一連のシステムセキュリティエンジニアリング活動とタスクを導入することは、必要な変化を開始するための重要な出発点および強制機能を提供する。

> “Providing satisfactory security controls in a computer system is in itself a system design problem. A combination of hardware, software, communications, physical, personnel and administrativeprocedural safeguards is required for comprehensive security. In particular, software safeguards alone are not sufficient.”
> 
> “Security Controls for Computer Systems,” (The Ware Report), Rand Corporation
> Defense Science Board Task Force on Computer Security, February 1970

「コンピュータシステムに満足のいくセキュリティコントロールを提供すること自体が、システム設計の問題である。包括的なセキュリティには、ハードウェア、ソフトウェア、通信、物理的、人事的および管理手続きのセーフガードの組み合わせが必要である。特に、ソフトウェアのセーフガードだけでは不十分である。」

> “Mission assurance requires systems that behave with predictability and proportionality.”
> 
> General Michael Hayden
> Former Director National Security Agency (NSA) and Central Intelligence Agency (CIA) Syracuse University,
October 2009

「ミッションの保証は、予測可能性と比例性を持って動作するシステムを必要とする。」

> “In the past, it has been assumed that to show that a system is safe, it is sufficient to provide assurance that the process for identifying the hazards has been as comprehensive as possible, and that each identified hazard has one or more associated controls. While historically this approach has been used reasonably effectively to ensure that known risks are controlled, it has become increasingly apparent that evolution to a more holistic approach is needed as systems become more complex and the cost of designing, building, and operating them become more of an issue.”
> 
> Preface, National Aeronautics and Space Administration (NASA) System Safety Handbook, Volume 1,
> November 2011

「過去には、システムが安全であることを示すためには、危険を特定するプロセスが可能な限り網羅的であったことを保証し、特定された各危険に一つ以上の関連するコントロールが存在することを示すことが十分であると考えられていた。このアプローチは歴史的に既知のリスクが管理されることを合理的に効果的に保証するために使用されてきたが、システムがより複雑になり、それらの設計、構築、運用のコストがより問題となるにつれて、より包括的なアプローチへの進化が必要であることが徐々に明らかになってきている。」

> “This whole economic boom in cybersecurity seems largely to be a consequence of poor engineering.”
> 
> Carl Landwehr
> Communications of the Association for Computing Machinery (ACM), February 2015

「このサイバーセキュリティにおける経済的なブームは、主に劣ったエンジニアリングの結果であるように思われる。」

> “Cybersecurity requires more than government action. Protecting our Nation from malicious cyber actors requires the Federal Government to partner with the private sector. The private sector must adapt to the continuously changing threat environment, ensure its products are built and operate securely, and partner with the Federal Government to foster a more secure cyberspace…Incremental improvements will not give us the security we need; instead, the Federal Government needs to make bold changes and significant investments in order to defend the vital institutions that underpin the American way of life.”
> 
> Executive Order (EO) on Improving the Nation’s Cybersecurity, May 2021

「サイバーセキュリティは、政府の行動だけでは足りない。我が国を悪意のあるサイバー行為者から守るためには、連邦政府が民間部門と提携する必要がある。民間部門は、絶えず変化する脅威環境に適応し、製品が安全に構築され、安全に運用されるようにし、より安全なサイバー空間を育成するために連邦政府と提携しなければならない…段階的な改善では、私たちが必要とするセキュリティを提供することはできない。その代わりに、連邦政府は大胆な変更と重要な投資を行う必要があり、アメリカの生活様式を支える重要な機関を守るために努力しなければならない。」

> “[Systems] security engineering must be fundamental to systems engineering, not just a specialty discipline. Security concepts must be fundamental to [an] engineering education, and security proficiency must be fundamental in development teams. Security fundamentals must be clearly understood by stakeholders and effectively evaluated in a way that considers broad goals with security functions and outcomes.”
> 
> Security in the Future of Systems Engineering (FuSE), a Roadmap of Foundational Concepts, INCOSE
> International Symposium, July 2021

「システムセキュリティエンジニアリングは、単なる専門分野ではなく、システムエンジニアリングの基本でなければならない。セキュリティの概念は、エンジニアリング教育の基本でなければならず、開発チームにおけるセキュリティの熟練度も基本でなければならない。セキュリティの基本は、利害関係者によって明確に理解され、セキュリティ機能と結果を考慮した方法で効果的に評価されなければならない。」

# Acknowledgments / 謝辞
The authors gratefully acknowledge and appreciate the significant contributions from individuals and organizations in the public and private sectors whose constructive comments improved the overall quality, thoroughness, and usefulness of this publication. In particular, we wish to thank Jeff Brewer, Ken Cureton, Jordan Denmark, Rick Dove, Holly Dunlap, Jim Foti, Michael Hankins, Daryl Hild, M. Lee, Tom Llanso, Jimmie McEver, Perri Nejib, Cory Ocker, Daniel Patrick Pereira, Victoria Pillitteri, Greg Ritter, Thom Schoeffling, Theresa Soloway, Nick Stegman, Gary Stoneburner, Gregory Touhill, Isabel Van Wyk, Adam Williams, Drew Wilson, Carol Woody, William Young, and Michael Zisa. The authors also wish to acknowledge members of the International Council for Systems Engineering (INCOSE), including members of the Systems Security Engineering and the Resilient Systems Working Groups, for numerous discussions on the content of the document. Finally, the authors wish to thank the students participating in INCOSE tutorials and MITRE Systems Security Engineering courses whose comments and valuable insights helped to guide and inform many of the proposed changes in this publication.

# Historical Contributions / 歴史的貢献
The authors gratefully acknowledge the contributions of Janet Carrier Oren, one of the original authors of NIST Special Publication 800-160, Volume 1. The authors also wish to acknowledge the following organizations and individuals for their historic contributions to this publication:

Organizations: National Security Agency; Naval Postgraduate School; Department of Defense Office of Acquisition, Technology, and Logistics; Department of Homeland Security Science and Technology Office, Cyber Security Division; International Council on Systems Engineering; United States Air Force; Air Force Institute of Technology; Northrop Grumman Corporation; The MITRE Corporation; The Boeing Company; Lockheed Martin Corporation.

Individuals: Beth Abramowitz, Max Allway, Kristen Baldwin, Dawn Beyer, Debora Bodeau, Paul Clark, Keesha Crosby, Judith Dahmann, Kelley Dempsey, Holly Dunlap, Jennifer Fabius, Daniel Faigin, Jeanne Firey, Robin Gandhi, Rich Graubart, Kevin Greene, Richard Hale, Daryl Hild, Kesha Hill, Danny Holtzman, Cynthia Irvine, Brett Johnson, Ken Kepchar, Stephen Khou,
Alvi Lim, Logan Mailloux, Dennis Mangsen, Doug Maughn, Rosalie McQuaid, Joseph Merkling, John Miller, Thuy Nguyen, Perri Nejib, Lisa Nordman, Dorian Pappas, Paul Popick, Roger Schell, Thom Schoeffling, Matthew Scholl, Peter Sell, Gary Stoneburner, Glenda Turner, Edward Yakabovicz, and William Young.

Finally, the authors respectfully acknowledge the seminal work in computer security that began in the 1960s. The vision, insights, and dedicated efforts of those early pioneers in computer security serve as the philosophical and technical foundation for the security principles, concepts, methods, and practices employed in this publication to address the critically important problem of engineering trustworthy secure systems.

# VIEWING SECURITY FROM THE PROPER PERSPECTIVE / 適切な視点からのセキュリティ観察
> “For the first few decades as a burgeoning discipline, cybersecurity has been dominated by the development of widgets to address some aspect of the problem. Systems have become increasingly complex and interconnected, creating even more attack opportunities, which in turn creates even more opportunities to create defensive widgets that will bring some value in detecting or preventing an aspect of the attack space. Eventually, this becomes a game of whack-a-mole in which a simulated mole pops up from one of many holes and the objective is to whack the mole before it pops back in its hole. The moles represent new attacks, and the holes represent a huge array of potential vulnerabilities – both known and as-yet-undiscovered.
> 
> Underlying [the discipline of] engineering is science. Sometimes engineering gets ahead of science, such as in bridge building, where the fundamentals of material science were not well understood. Many bridges were built; many fell down; some stayed up; designs of the ones that stayed up were copied. Eventually, for engineering to advance beyond some point, science must catch up with engineering. The science underlying cybersecurity [and more generally, security] engineering is complex and difficult. On the other hand, there is no time like the present to start, because it is both urgent and important to the future.…”
> 
> -- O. Sami Saydjari
>  Engineering Trustworthy Systems McGraw-Hill, August 2018

「サイバーセキュリティが成長していく新興分野としての最初の数十年間、問題のある側面に対処するためのウィジェットの開発が支配的であった。システムはますます複雑で相互接続され、さらに多くの攻撃機会を生み出し、それがさらに防御ウィジェットを作成する機会を生み出す。これらのウィジェットは、攻撃空間のある側面を検出または防止する価値をもたらす。最終的には、これはモグラたたきのゲームとなり、シミュレートされたモグラが多くの穴の1つから現れ、そのモグラが穴に戻る前にたたくことが目的となる。モグラは新しい攻撃を表し、穴は既知のものもまだ発見されていないものも含む膨大な潜在的脆弱性を表す。

エンジニアリングの基盤には科学がある。時にはエンジニアリングが科学を先取りすることがあり、例えば橋の建設では、材料科学の基本が十分に理解されていなかった。多くの橋が建設され、多くが崩壊し、いくつかは残った。残ったものの設計はコピーされた。最終的に、エンジニアリングがある点を超えて進むためには、科学がエンジニアリングに追いつかなければならない。サイバーセキュリティ（そしてより一般的にはセキュリティ）エンジニアリングの基盤となる科学は複雑で難しい。一方で、始めるには今が最適な時期である。なぜなら、それは未来にとって緊急かつ重要だからである…。」

# THE IMPORTANCE OF SCIENCE AND ENGINEERING / 科学とエンジニアリングの重要性
> When crossing a bridge, we have a reasonable expectation that the bridge will not collapse and will get us to our destination without incident. For bridge builders, the focus is on equilibrium, static and dynamic loads, vibrations, and resonance. The science of physics combines with civil engineering principles and concepts to produce a product that we deem trustworthy, giving us a level of confidence that the bridge is fit-for-purpose.

橋を渡る際、私たちはその橋が崩れることなく、何の問題もなく目的地に着くという合理的な期待を持っている。橋の建設者にとって、焦点は平衡、静的および動的荷重、振動、共鳴にある。物理学の科学は土木工学の原理と概念と組み合わさり、私たちが信用できると判断する製品を生み出す。これにより、橋が目的に適しているという信頼感が得られる。

> For system developers, there are also fundamental principles and concepts that can be found in mathematics, computer science, computer and electrical engineering, systems engineering, and software engineering that when properly employed, provide the necessary trustworthiness to engender that same level of confidence.

システム開発者にとっても、数学、コンピュータサイエンス、コンピュータおよび電気工学、システムエンジニアリング、ソフトウェアエンジニアリングにおいて見出される基本的な原理と概念があり、これらが適切に用いられることで、必要な信用度を提供し、同じレベルの信頼感を生み出す。

> Trustworthy secure systems are achieved by making a significant and substantial investment in strengthening the underlying systems and system components by employing transdisciplinary systems engineering efforts guided and informed by welldefined security requirements and secure architectures and designs. Such efforts have been proven over time to produce sound engineering-based solutions to complex and challenging systems security problems. Only under those circumstances can we build systems that are adequately secure and exhibit a level of trustworthiness that is sufficient for the purpose for which the system was built.

信用度の高い安全なシステムは、よく定義されたセキュリティ要件と安全なアーキテクチャおよび設計によって導かれ、情報提供される学際的なシステムエンジニアリングの努力を用いて、基礎となるシステムおよびシステムコンポーネントを強化するための重要かつ実質的な投資によって達成される。このような努力は、時間をかけて複雑で難しいシステムセキュリティの問題に対する健全な工学ベースの解決策を生み出すことが証明されている。これらの状況の下でのみ、私たちは適切に安全で、システムが構築された目的に十分な信用度を示すシステムを構築することができる。

> “Scientists study the world as it is, engineers create the world that never has been.”
> 
> Theodore von Kármán
> 1962 National Medal of Science Recipient

「科学者はあるがままの世界を研究するが、エンジニアはこれまでになかった世界を創造する。」

# CRITICAL SYSTEM BEHAVIORS OF THE FUTURE / 未来における重要システムの振る舞い
> “To deliver system behavior, the systems engineer must define a group of subsystems and precisely how those subsystems are to interact with each other. It is the subsystems and their interactions which produce the system-level behavior. Many of us recognize a vehicle that can take a 60-degree curve at 200 miles per hour as possessing a valuable system behavior. Would we as quickly recognize safe, private, trusted, and available as system behaviors? These behaviors require the same careful system-level design and trades to achieve optimal solutions as the performance system behavior I mentioned above. And there is a clear need — investors want the system to keep their data private, to be safe, and to be trustworthy so that their control is not compromised by a cyber threat, and to be highly available.
> 
> If we systems engineers are willing to recognize these behaviors as system behaviors, then we are accountable for delivering them as part of our job. If we choose to view these behaviors as attributes of the parts of our system but not the system as a whole, then we are likely to consider them as jobs for the “specialty engineers.” I’ve looked back into past behaviors of our system engineering community. What I find are examples of systems engineers giving our ‘specialty engineering’ colleagues these challenges by way of the requirements-allocation process. I think we have been wrong to do this. Our “specialty” colleagues are likely to take these allocated requirements and focus on building safe, private, trusted, available parts of a system—rather than in delivering safe, private, trusted, and available system behaviors. It is true you can build a safer system by building safe parts. However, you can’t build a truly safe system without having safe parts interacting with each other in a safe manner. The same can be said for other system behaviors (private, trusted, available, and so on).”
> 
> -- John A. Thomas
>  President, INCOSE
>  INCOSE Insight, July 2013.

「システムの振る舞いを実現するために、システムエンジニアは一群のサブシステムを定義し、それらのサブシステムが互いにどのように相互作用するかを正確に決めなければならない。システムレベルの振る舞いを生み出すのは、これらのサブシステムとその相互作用である。多くの人々は、60度のカーブを時速200マイルで曲がることができる車両を、価値あるシステムの振る舞いを持つものと認識する。しかし、安全で、プライベートで、信頼され、利用可能なものをシステムの振る舞いとしてすぐに認識するだろうか？これらの振る舞いは、私が上述した性能システムの振る舞いと同様に、最適な解決策を達成するための慎重なシステムレベルの設計とトレードオフを必要とする。そして、明らかなニーズがある―投資家たちは、システムがデータをプライベートに保ち、安全で、信頼できること、つまりサイバー脅威によってコントロールが妥協されないこと、そして高い可用性を持つことを望んでいる。

もし私たちシステムエンジニアがこれらの振る舞いをシステムの振る舞いとして認識する意志があるなら、私たちはそれらを私たちの仕事の一部として提供する責任がある。これらの振る舞いをシステムの一部としてではなく、システム全体として見ることを選ぶなら、私たちはそれらを「専門のエンジニア」の仕事と考える可能性が高い。私は私たちのシステムエンジニアリングコミュニティの過去の振る舞いを振り返ってみた。そこで見つけたのは、システムエンジニアが要件割り当てプロセスを通じて「専門エンジニアリング」の同僚にこれらの課題を与えている例である。これを行うことは間違っていたと思う。私たちの「専門」の同僚は、これらの割り当てられた要件を受け取り、安全で、プライベートで、信頼され、利用可能なシステムの部分を構築することに焦点を当てることが多い―安全で、プライベートで、信頼され、利用可能なシステムの振る舞いを提供するというよりも。安全な部品を構築することでより安全なシステムを構築することは可能であるが、安全な部品が互いに安全な方法で相互作用することなく、本当に安全なシステムを構築することはできない。これは他のシステムの振る舞い（プライベート、信頼、利用可能など）についても同様である。」
