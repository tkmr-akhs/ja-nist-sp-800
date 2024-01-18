# Introduction / はじめに
> Today's systems[^1] are inherently complex. The growth in the size, number, and types of components and technologies[^2] that compose those systems as well as the system dependencies result in a range of consequences from inconvenience to catastrophic loss due to adversity[^3] within the operating environment. Managing the complexity of trustworthy secure systems requires achieving the appropriate level of confidence in the feasibility, correctness-in-concept, philosophy, and design of a system to produce only the intended behaviors and outcomes. This provides the foundation to address stakeholder protection needs and security concerns with sufficient confidence that the system functions only as intended while subjected to different types of adversity and to realistically bound those expectations with respect to constraints and uncertainty. The failure to address complexity and security will leave the Nation susceptible to potentially serious, severe, or catastrophic consequences.

今日のシステム[^1j]は本質的に複雑である。 これらのシステムを構成するコンポーネントやテクノロジー[^2j]のサイズ、数、種類の増大とシステムの依存関係は、動作環境内での不便から逆境による壊滅的な損失に至るまで、さまざまな影響を及ぼす[^3j]。 。 信頼できる安全なシステムの複雑さを管理するには、意図した動作と結果のみを生み出すシステムの実現可能性、コンセプトの正しさ、哲学、設計において適切なレベルの信頼を達成する必要がある。 これにより、さまざまな種類の逆境にさらされている間でもシステムが意図したとおりにのみ機能し、制約や不確実性に関してそれらの期待を現実的に拘束できるという十分な自信を持って、ステークホルダーの保護のニーズとセキュリティ上の懸念に対処するための基盤が提供される。 複雑さと安全性に対処できなければ、この国は潜在的に深刻な、重大な、または破滅的な結果にさらされることになる。

> The term security is used in this publication to mean freedom from the conditions that can cause a loss of assets with unacceptable consequences.[^4] Stakeholders must define the scope of security in terms of the assets to which security applies and the consequences against which security is assessed.[^5] Systems engineering provides a foundation for a disciplined and structured approach to building assured, trustworthy secure systems. As a systems engineering subdiscipline, systems security engineering addresses security-relevant considerations intended to produce secure outcomes. The engineering efforts are conducted at the appropriate level of fidelity and rigor needed to achieve trustworthiness and assurance objectives.

本書では、セキュリティという用語は、容認できない結果を伴う資産の損失を引き起こす可能性のある条件から解放されることを意味するために使用されている。[^4j] 利害関係者は、セキュリティが適用される資産とその影響に関してセキュリティの範囲を定義する必要がある。 [^5j] システム エンジニアリングは、確実で信頼できる安全なシステムを構築するための、規律正しく構造化されたアプローチの基礎を提供する。 システム セキュリティ エンジニアリングは、システム エンジニアリングの下位分野として、安全な結果を生み出すことを目的としたセキュリティ関連の考慮事項に取り組みます。 エンジニアリングの取り組みは、信用度と保証 (assurance) の目的を達成するために必要な、適切なレベルの忠実性と厳格さで実行される。

[^1]: A system is an arrangement of parts or elements that exhibit a behavior or meaning that the individual constituents do not [3]. The elements that compose a system include hardware, software, data, humans, processes, procedures, facilities, materials, and naturally occurring entities [4].

[^1j]: システムとは、個々の構成要素は持たない動作や意味を示す部品や要素の配置である [3]。 システムを構成する要素には、ハードウェア、ソフトウェア、データ、人間、プロセス、手順、設備、材料、自然発生物が含まれる [4]。

[^2]: The term technology is used in the broadest context in this publication to include computing, communications, and information technologies, as well as any mechanical, hydraulic, pneumatic, or structural components in systems that contain or are enabled by such technologies. This view of technology provides an increased recognition of the digital, computational, and electronic machine-based foundation of modern complex systems and the growing importance of an assured trustworthiness of that foundation in providing the system's functional capability and interaction with its physical machine and human system elements.

[^2j]: 本書では、「技術」という言葉は、コンピューティング、通信、情報技術だけではなく、そのような技術を含む、あるいは、それらによって可能となるシステムの機械的、油圧的、空気圧的、または建造的なコンポーネントまでをも含む、最も広い文脈で使用される。この「技術」の視点は、デジタル、計算的、電子的な機械に基づく、現代の複雑なシステムの基礎に関する、より高められた認識を提供し、また、システムの機能的な能力とそのシステムの物理的機械および人間のシステム要素との相互作用の提供における、そのシステムの基礎の保証された信頼性をより重要なものにする。(なにをいってるかよくわからんうえに、ぶんがながすぎて、ほんやくできない)

[^3]: The term adversity refers to those conditions that can cause asset loss (e.g., threats, attacks, vulnerabilities, hazards, disruptions, and exposures).

[^3j]: 「逆境」という言葉は、資産の損失を引き起こす可能性がある状況を指します（例えば、脅威、攻撃、脆弱性、危険、混乱、露出など）。

[^4]: The phrasing used in this definition of security is intentional. Ross Anderson noted in [5] that “now that everything’s acquiring connectivity, you can’t have safety without security, and these ecosystems are emerging.” Reflecting on this observation, the security definition was chosen to achieve alignment with a prevailing safety definition.

[^4j]: このセキュリティの定義で使用されている言い回しは意図的なものである。Ross Anderson は [5] で「今や全てが接続性を獲得しているため、セキュリティなしに安全はあり得ず、これらのエコシステムが出現している」と指摘した。この観察を反映して、セキュリティの定義は一般的な安全の定義との整合性を図るために選ばれた。

[^5]: > Adapted from [6].

[^5j]: [6] から改変。

Peter Neumann described the concept of trustworthiness in [2] as follows:

“By trustworthiness, we mean simply worthy of being trusted to fulfill whatever critical requirements may be needed for a particular component, subsystem, system, network, application, mission, enterprise, or other entity. Trustworthiness requirements might typically involve (for example) attributes of security, reliability, performance, and survivability under a wide range of potential adversities. Measures of trustworthiness are meaningful only to the extent that (a) the requirements are sufficiently complete and well defined, and (b) can be accurately evaluated.”

Systems security engineering provides complementary engineering capabilities that extend the concept of trustworthiness to deliver trustworthy secure systems. Trustworthiness is not only about demonstrably meeting a set of requirements. The requirements must also be complete, consistent, and correct. From a security perspective, a trustworthy system meets a set of welldefined requirements, including security requirements. Through evidence and expert judgment, trustworthy secure systems can limit and prevent the effects of modern adversities. Such adversities come in malicious and non-malicious forms and can emanate from a variety of sources, including physical and electronic. Adversities can include attacks from determined and capable adversaries, human errors of omission and commission, accidents and incidents, component faults and failures, abuses and misuses, and natural and human-made disasters.

## Purpose and Applicability / 目的と適用範囲
This publication is intended to:
* Provide a basis for establishing a discipline for systems security engineering as part of systems engineering in terms of its principles, concepts, activities, and tasks
* Foster a common mindset to deliver security for any system, regardless of its purpose, type, scope, size, complexity, or stage of the system life cycle
* Demonstrate how selected systems security engineering principles, concepts, activities, and tasks can be effectively applied to systems engineering activities
* Advance the field of systems security engineering as a discipline that can be applied and studied
* Serve as a basis for the development of educational and training programs, including individual certifications and other professional assessment criteria

The considerations set forth in this publication are applicable to all federal systems other than those systems designated as national security systems as defined in 44 U.S.C., Section 3542.[^6] These considerations have been broadly developed from a technical and technical management perspective to complement similar considerations for national security systems and may be used for such systems with the approval of federal officials who exercise policy authority over such systems. State, local, and tribal governments, as well as private sector entities, are encouraged to consider using the material in this publication, as appropriate.

[^6]: Increasing the trustworthiness of systems is a significant undertaking that requires a substantial investment in the requirements, architecture, design, and development of systems, system components, applications, and networks. The policy in [8] requires federal agencies to implement the systems security engineering principles, concepts, techniques, and system life cycle processes in this publication for all high-value assets.  “Security is embedded in systems. Rather than two engineering groups designing two systems, one intended to protect the other, systems engineering specifies and designs a single system with security embedded in the system and its components.”  -- An Objective of Security in the Future of Systems Engineering [7]

[^6j]: システムの信用度を高めることは、システム、システムコンポーネント、アプリケーション、ネットワークの要件、アーキテクチャ、設計、開発において相当な投資を必要とする重要な取り組みである。[8]の方針では、連邦機関に対して、本書のシステムセキュリティエンジニアリングの原則、概念、技術、システムライフサイクルプロセスを全ての高価値資産に対して実施することを要求している。  「セキュリティはシステムに組み込まれている。他を守ることを目的とした2つのシステムを設計する2つのエンジニアリンググループではなく、システムエンジニアリングは、システムとそのコンポーネントにセキュリティを組み込んだ単一のシステムを指定し設計する。」  -- An Objective of Security in the Future of Systems Engineering [7]

> The applicability statement is not meant to limit the technical and management application of these considerations. That is, the security design principles, concepts, and techniques described in this publication are part of a trustworthy secure design approach as described in Appendix D and can be applied in any of the following cases:

適用性の声明は、これらの考慮事項の技術的および管理的応用を制限するものではない。つまり、本書に記述されているセキュリティ設計の原則、概念、および技術は、付録Dに記述されているような信用度の高い安全な設計アプローチの一部であり、次のいずれかの場合に適用可能である：

> * Development of a new capability or system
>   * The engineering effort includes such activities as concept exploration, preliminary or applied research to refine the concepts and/or feasibility of technologies employed in a new system, and an assessment of alternative solutions. This effort is initiated during the concept and development stages of the system life cycle.

* 新しい機能またはシステムの開発
  * このエンジニアリングの取り組みには、概念の探求、新しいシステムで使用される技術の概念および/または実現可能性を洗練させるための予備的または応用研究、代替解決策の評価などの活動が含まれる。この努力は、システムライフサイクルの概念および開発段階で開始される。

> * Modification of an existing capability or system
>   * Reactive modifications to fielded systems: The engineering effort occurs in response to adversity that diminishes or prevents the system from achieving the design intent. This effort can occur during the production, utilization, or support stages of the system life cycle and may be performed concurrently with or independent of day-to-day system operations.
>   * Planned upgrades to fielded systems while continuing to sustain day-to-day operations: Planned system upgrades may enhance an existing system capability, provide a new capability, or constitute a technology refresh of an existing capability. This effort occurs during the production, utilization, or support stages of the system life cycle.
>   * Planned upgrades to fielded systems that result in new systems: The engineering effort is conducted as if developing a new system with a system life cycle that is distinct from the life cycle of a fielded system. The upgrades are performed in a development environment that is independent of the fielded system.

* 既存の機能またはシステムの変更
  * 実装済みシステムへのリアクティブな変更：エンジニアリングの取り組みは、設計意図を達成することを減少させるか阻害する逆境に応じて行われる。この努力は、システムライフサイクルの製造、利用、またはサポート段階で発生し、日々のシステム運用と並行して、またはそれとは独立して実施される場合がある。
  * 日々の運用を継続しながらの実装済みシステムへの計画的なアップグレード：計画されたシステムアップグレードは、既存のシステム機能を向上させたり、新しい機能を提供したり、既存の機能の技術更新を行うことがある。この努力は、システムライフサイクルの製造、利用、またはサポート段階で発生する。
  * 新しいシステムをもたらす実装済みシステムへの計画的なアップグレード：エンジニアリングの取り組みは、新しいシステムを開発するかのように行われ、そのシステムライフサイクルは実装済みシステムのライフサイクルとは異なる。アップグレードは、実装済みシステムから独立した開発環境で実施される。

> * Evolution of an existing capability or system
>   * The engineering effort involves migrating or adapting a system or system implementation from one operational environment or set of operating conditions to another operational environment or set of operating conditions.[^7]

* 既存の機能またはシステムの進化
  * エンジニアリングの取り組みには、システムまたはシステムの実装をある運用環境または運用条件から別の運用環境または運用条件に移行または適応させることが含まれる。[^7j]

> * Retirement of an existing capability or system
>   * The engineering effort removes system functions, services, elements, or the entire system from operation and may include the transition of system functions and services to another system. The effort occurs during the retirement stage of the system life cycle and may be conducted while sustaining day-to-day operations.

* 既存の機能またはシステムの退役
  * エンジニアリングの取り組みは、システムの機能、サービス、要素、またはシステム全体を運用から除去し、システムの機能とサービスを別のシステムに移行することも含むことがある。この努力は、システムライフサイクルの退役段階で行われ、日々の運用を維持しながら実施されることがある。

> * Development of a dedicated, domain-specific, or special-purpose capability or system
>   * Security-dedicated or security-purposed system: The engineering effort delivers a system that satisfies a security-dedicated need or provides a security-oriented purpose and does so as a stand-alone system that may monitor or interact with other systems. Such systems can include surveillance systems, physical protection systems, monitoring systems, and security service provisioning systems.
>   * High-confidence, dedicated-purpose system: The engineering effort delivers a system that satisfies the need for real-time vehicular control, industrial or utility processes, weapons, nuclear power plants, and other special-purpose needs. Such systems may include multiple operational states or modes with varying forms of manual, semi-manual, automated, or autonomous modes. These systems have highly deterministic properties, strict timing constraints, functional interlocks, and severe or catastrophic consequences of failure.

* 専用、ドメイン特化、特定目的の機能またはシステムの開発
  * セキュリティ専用またはセキュリティ目的のシステム：エンジニアリングの取り組みは、セキュリティ専用のニーズを満たすまたはセキュリティ指向の目的を提供するシステムを提供し、他のシステムを監視または対話する単独のシステムとして行う。これらのシステムには、監視システム、物理的保護システム、監視システム、セキュリティサービス提供システムなどが含まれる。
  * 高信頼性、専用目的のシステム：エンジニアリングの取り組みは、リアルタイムの車両制御、産業または公共事業プロセス、兵器、原子力発電所、その他の特定目的のニーズに対するシステムを提供する。これらのシステムには、手動、半手動、自動化、自律的なモードを含む複数の運用状態またはモードが含まれることがある。これらのシステムは高度に決定論的な特性、厳格なタイミング制約、機能的インターロック、および失敗の重大または壊滅的な結果を持つ。

> * Development of a system of systems
>   * The engineering effort occurs across a set of constituent systems, each with its own stakeholders, primary purpose, and planned evolution. The composition of the constituent systems into a system of systems as noted in [9] produces a capability that would otherwise be difficult or impractical to achieve. This effort can occur across a variety of system of systems from a relatively informal, unplanned system of systems concept and evolution that emerges over time via voluntary participation to a more formal execution with the most formal being a system of systems concept that is directed, structured, planned, and achieved via a centrally managed engineering effort. Any resulting emergent behavior often introduces opportunities and additional challenges for systems security engineering.

* システム・オブ・システムズの開発 
  * エンジニアリングの取り組みは、それぞれ独自の利害関係者、主要目的、計画された進化を持つ一連の構成システム間で行われる。構成システムをシステム・オブ・システムズに組み合わせることは、それ以外では困難または非現実的である機能を生み出す。この取り組みは、自発的な参加によって時間をかけて自然に発生する比較的非公式で計画されていないシステム・オブ・システムズの概念と進化から、最も公式なものである中央管理されたエンジニアリングの取り組みを通じて指示され、構造化され、計画され、達成される

## Target Audience / 対象読者
> This publication is intended for systems engineers, security engineers, and other engineering professionals. The term systems security engineer is used to include systems engineers and security professionals who apply the concepts and principles and perform the activities and tasks described in this publication.[^8] This publication can also be used by professionals who perform other system life cycle activities or tasks, including:

本書は、システムエンジニア、セキュリティエンジニア、およびその他のエンジニアリング専門家を対象としている。用語「システムセキュリティエンジニア」は、本書に記述されている概念と原則を適用し、活動とタスクを実行するシステムエンジニアおよびセキュリティ専門家を含むために使用される。本書は、他のシステムライフサイクルの活動やタスクを実行する専門家にも使用されることができる。これには以下のようなものが含まれる：

> * Individuals with security governance, risk management, and oversight responsibilities

セキュリティガバナンス、リスク管理、監督責任を持つ個人

> * Individuals with security verification, validation, testing, evaluation, auditing, assessment, inspection, and monitoring responsibilities

セキュリティの検証、検証、テスト、評価、監査、評価、検査、監視の責任を持つ個人

> * Individuals with acquisition, budgeting, and project management responsibilities

購入、予算編成、プロジェクト管理の責任を持つ個人

> * Individuals with operations, maintenance, sustainment, logistics, and support responsibilities

運用、保守、維持、物流、サポートの責任を持つ個人

> * Providers of technology-related products, systems, or services

技術関連の製品、システム、またはサービスを提供する事業者

> * Educators in academic institutions that offer systems engineering, computer engineering, computer science, software engineering, and computer security programs

システムエンジニアリング、コンピュータエンジニアリング、コンピュータサイエンス、ソフトウェアエンジニアリング、コンピュータセキュリティプログラムを提供する学術機関の教育者

[^7]: There is a growing need to reuse or leverage system implementation successes within operational environments that are different from how they were originally designed and developed. This type of reuse or reimplementation of systems within other operational environments is more efficient and represents potential advantages in maximizing interoperability between various system implementations. It should be noted that reuse may violate the assumptions used to determine that a system or system component was trustworthy.

[^7j]: 運用環境が元の設計や開発と異なる場合に、システム実装の成功を再利用または活用する必要性が高まっている。このような再利用または他の運用環境でのシステムの再実装は、効率的であり、さまざまなシステム実装間の相互運用性を最大化する潜在的な利点を表している。ただし、再利用がシステムまたはシステムコンポーネントが信用度のあると判断された前提を破る可能性があることに注意すべきである。

[^8]: Systems security engineering activities and tasks can be applied to a mechanism, component, system element, system, system of systems, processes, or organizations. Regardless of the size or complexity of the entity, a transdisciplinary systems engineering team is needed to deliver systems that are trustworthy and that satisfy the protection needs and concerns of stakeholders. The processes are intended to be tailored to facilitate effectiveness.

[^8j]: システムセキュリティエンジニアリングの活動とタスクは、メカニズム、コンポーネント、システム要素、システム、システム・オブ・システムズ、プロセス、または組織に適用することができる。エンティティのサイズや複雑さに関わらず、信用度の高いシステムを提供し、利害関係者の保護ニーズと懸念を満たすためには、学際的なシステムエンジニアリングチームが必要である。プロセスは、効果を促進するためにカスタマイズされることを意図している。

## How to Use this Publication / 本書の使い方
> This publication is intended to serve as a reference and educational resource for systems engineers, engineering specialties, architects, designers, and any individuals involved in the development of trustworthy secure systems and system components. It is meant to be flexible in its application to meet the diverse needs of organizations. There is no expectation that all of the technical content in this publication will be used as part of a systems engineering effort. Rather, the concepts and principles for trustworthy secure design in Appendices D through F as well as the systems life cycle processes and security-relevant activities and tasks in Appendices G through K can be selectively employed by organizations – relying on the experience and expertise of the engineering teams to determine what is correct for their purposes. Applying the content of this publication enables the achievement of security outcomes that are consistent with the systems engineering perspective on system life cycle processes.

本書は、システムエンジニア、エンジニアリングの専門家、アーキテクト、デザイナー、信用度の高い安全なシステムおよびシステムコンポーネントの開発に関わるすべての個人に対する参考資料および教育資源として機能することを意図している。それは、組織の多様なニーズに応えるためにその応用が柔軟であることを意味している。本書の全ての技術内容がシステムエンジニアリングの努力の一部として使用されるとは期待されていない。むしろ、付録DからFに記載されている信用度の高い安全な設計のための概念と原則、および付録GからKに記載されているシステムライフサイクルプロセスとセキュリティ関連の活動とタスクは、組織によって選択的に採用されることができる。これは、エンジニアリングチームの経験と専門知識に依存し、それらの目的にとって何が正しいかを決定する。本書の内容を適用することにより、システムライフサイクルプロセスに対するシステムエンジニアリングの観点と一致するセキュリティ成果の達成が可能になる。

> The system life cycle processes described in this publication can take advantage of any system or software development methodology. The processes are equally applicable to waterfall, spiral, DevOps, agile, and other approaches. The processes can be applied recursively, iteratively, concurrently, sequentially, or in parallel and to any system regardless of its size, complexity, purpose, scope, operational environment, or special nature. The full extent of the application of the content in this publication is guided by stakeholder capability needs, protection needs, and concerns with particular attention paid to considerations of cost, schedule, and performance.

この出版物に記述されたシステムライフサイクルプロセスは、どのようなシステムまたはソフトウェア開発方法論を利用することもできる。これらのプロセスは、ウォーターフォール、スパイラル、DevOps、アジャイル、その他のアプローチに等しく適用可能である。プロセスは再帰的に、反復的に、同時に、逐次的に、または並列に適用することができ、そのサイズ、複雑さ、目的、範囲、運用環境、特別な性質に関係なく、どのようなシステムにも適用可能である。この出版物の内容の適用の全範囲は、利害関係者の能力ニーズ、保護ニーズ、特にコスト、スケジュール、性能の考慮事項に特に注意を払いながら、懸念事項によって導かれる。

## Organization of this Publication / 本書の構成
> The remainder of this publication is organized as follows:

本書の残りの部分は、以下のように構成されている：

> * Chapter 2 presents an overview of systems engineering and the fundamental concepts associated with engineering trustworthy secure systems. This includes basic concepts that address the structure and types of systems, systems engineering foundations, and the concepts of trust and trustworthiness of systems and system components.

* 第2章では、システムエンジニアリングと、信用度の高いセキュアなシステムをエンジニアリングする際の基本概念についての概要を提示する。これには、システムの構造とタイプ、システムエンジニアリングの基礎、そしてシステム及びシステムコンポーネントの信用度と信頼性に関する基本概念が含まれる。

> * Chapter 3 describes foundational system security concepts and an engineering perspective to building trustworthy secure systems. This includes the concepts of security and system security, the nature and character of systems, the concepts of assets and asset loss, reasoning about asset loss, defining protection needs, system security viewpoints, demonstrating system security, and an introduction to systems security engineering.

* 第3章では、基本的なシステムセキュリティ概念と、信用度の高いセキュアなシステムを構築するためのエンジニアリングの視点を説明する。これには、セキュリティとシステムセキュリティの概念、システムの性質と特性、資産と資産損失の概念、資産損失に関する推論、保護ニーズの定義、システムセキュリティの視点、システムセキュリティの実証、およびシステムセキュリティエンジニアリングへの導入が含まれる。

> * Chapter 4 provides a systems security engineering framework that includes a problem context, solution context, and trustworthiness context.

* 第4章では、問題の文脈、解決策の文脈、及び信用度の文脈を含むシステムセキュリティエンジニアリングフレームワークを提供する。

> The following sections provide additional information to support the engineering of trustworthy secure systems:

以下のセクションでは、信用度の高い安全なシステムのエンジニアリングをサポートするための追加情報を提供する：

> * References
>   * Appendix A: Acronyms / アクロニム
>   * Appendix B: Glossary / 用語集
>   * Appendix C: Security Policy and Requirements / セキュリティ ポリシーと要件
>   * Appendix D: Trustworthy Secure Design / 信用度の高いセキュアな設計
>   * Appendix E: Principles for Trustworthy Secure Design / 信用度の高いシステムのための設計アプローチ
>   * Appendix F: Trustworthiness and Assurance / 信用度と保証
>   * Appendix G: System Life Cycle Processes Overview / システムライフサイクルプロセスの概要
>   * Appendix H: Technical Processes / 技術的プロセス
>   * Appendix I: Technical Management Processes / 技術的マネジメントプロセス
>   * Appendix J: Organizational Project-Enabling Processes / 組織的なプロジェクト実現プロセス
>   * Appendix K: Agreement Processes / 契約プロセス
>   * Appendix L: Change Log / 更新履歴

## ENGINEERING-DRIVEN SOLUTIONS / エンジニアリング主導のソリューション
> The effectiveness of any engineering discipline first requires a thorough understanding of the problem and consideration of all feasible solutions before acting to solve the identified problem. To maximize the effectiveness of systems security engineering, the security requirements for the protection against asset loss must be driven by business, mission, and all other stakeholder asset loss concerns.

> The security requirements are defined and managed as a well-defined set of engineering requirements and cannot be addressed independently or after the fact.

> In the context of systems security engineering, the term protection has a broad scope and is primarily focused on the concept of assets and asset loss resulting in unacceptable consequences. The protection capability provided by a system goes beyond prevention and aims to control the events, conditions, and consequences that constitute asset loss. It is achieved in the form of the specific capability and constraints on system architecture, design, function, implementation, construction, selection of technology, methods, and tools and must be “engineered in” as part of the system life cycle process.

Understanding stakeholder asset protection needs (including assets that they own and assets that they do not own but must protect) and expressing those needs through a set of well-defined security requirements is an investment in the organization’s mission and business success in the modern age of global commerce, powerful computing systems, and network connectivity.
