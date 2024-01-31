# Appendix F. Trustworthiness and Assurance / 信用性と保証
> The trustworthiness of a system is based on the concept of assurance. Assurance is the grounds for justified confidence that a claim or set of claims has been or will be achieved [61]. Justified confidence is derived from objective evidence that reduces uncertainty to an acceptable level and, in doing so, reduces the associated risk (Section F.2).[^85] Evidence is produced by engineering verification and validation methods.[^86] The evidence must be relevant, accurate, credible, and of sufficient quantity to enable reasoned conclusions and consensus among subjectmatter experts that the claims are satisfied. The relationship between evidence and claims can be represented in many ways. Section F.2 discusses these approaches.

システムの信用性は、保証という概念に基づいている。保証とは、ある主張または一連の主張が達成された、あるいは達成されるという正当な確信の根拠である[61]。正当な確信は、不確実性を受け入れられるレベルまで減少させ、それによって関連するリスクを減少させる客観的証拠から導かれる（セクションF.2）[^85j]。証拠は、エンジニアリングの検証と妥当性確認の方法によって生成される[^86j]。証拠は、関連性があり、正確で、信頼できるものでなければならず、また、主張が満たされているという合理的な結論に至り、専門家間でのコンセンサスを可能にするための十分な量でなければならない。証拠と主張との関係は、多くの方法で表現されることがある。セクションF.2では、これらのアプローチについて議論している。

> “The trust we place in our digital infrastructure should be proportional to how trustworthy and transparent that infrastructure is and to the consequences we will incur if that trust is misplaced.”
> 
> -- Executive Order (EO) on Improving the Nation’s Cybersecurity [1]  May 2021 

「私たちがデジタルインフラに置く信用は、そのインフラがどれだけ信用できるか、そして透明であるか、またその信用が誤っていた場合に私たちが負うであろう結果に比例すべきである。」

[^85]: > This includes risks attributed to poor, incorrect, and unjustified decisions.

[^85j]: これには、不十分な、誤った、そして根拠のない決定に起因するリスクが含まれる。

[^86]: > These methods include combinations of demonstration, inspection, analysis, and testing.

[^86j]: これらの方法には、実証、検査、分析、およびテストの組み合わせが含まれる。

## F.1. Trust and Trustworthiness / 信用と信用性
> As discussed in Section 2.3, trust and trustworthiness are foundational concepts to engineering trustworthy secure systems, to the decisions made to grant trust, and to the extent to which trust is granted based on demonstrated trustworthiness. Trust is a belief that an entity meets certain expectations and can, therefore, be relied upon. A trustworthy entity requires sufficient evidence to support its trustworthiness claims. Trustworthiness is demonstrated based on evidence that supports a stated claim or judgment of being worthy to be trusted [2] [20] [21].

セクション2.3で議論されているように、信用と信用性は、信用に値する安全なシステムをエンジニアリングするための基本的な概念であり、信用を与えるための決定、および実証された信用性に基づいて信用がどの程度与えられるかに関連している。信用とは、あるエンティティが特定の期待を満たすという信念であり、したがって、信頼することができる。信用に値するエンティティは、その信用性の主張を支持する十分な証拠を必要とする。信用性は、信用するに値するという主張や判断を支持する証拠に基づいて実証される[2] [20] [21]。

> Trust in an entity can occur without a basis for or knowledge of the entity’s trustworthiness. This may occur because (1) there is no alternative (e.g., an individual trusts the components involved in an Internet transaction without knowing anything about the components), (2) the need for trustworthiness is not realized and occurs de facto, or (3) other reasons (e.g., miscommunication or misrepresentation of evidence) [58]. Since the decision to trust an entity is not necessarily based on a judgment of trustworthiness, the decision to trust an entity should consider the significance (i.e., consequences, effects, and impacts) of trust expectations not being fulfilled.

エンティティに対する信用は、そのエンティティの信用性の根拠や知識がなくても生じることがある。これは、（1）代替がない場合（例えば、個人がインターネット取引に関わるコンポーネントを、そのコンポーネントについて何も知らないまま信用する）、（2）信用性が必要であると認識されず、事実上信用される場合、または（3）その他の理由（例えば、証拠の誤伝達や誤表現）によって生じることがある[58]。エンティティを信用するという決定は必ずしも信用性の判断に基づいているわけではないため、エンティティを信用する決定は、信用の期待が満たされないことの重要性（つまり、結果、影響、及びインパクト）を考慮すべきである。

> The criteria to grant trust are used to determine the trustworthiness of an entity. Trust granted without establishing the required trustworthiness is a significant contributor to risk.

信用を与えるための規準は、エンティティの信用性を決定するために使用される。必要な信用性を確立せずに与えられた信用は、リスクの重要な要因である。

### F.1.1. Roles of Requirements in Trustworthiness / 信用性における要件の役割
> Trustworthiness judgments are based on expectations to be fulfilled by the entity to be trusted.
The expectations of trustworthiness of the system, inclusive of its elements, are found in the system capability, performance, security, and other requirements. These judgments are meaningful only to the extent to which the trustworthiness-relevant requirements accurately reflect the problem, accurately define the solution, and can be verified as being satisfied by the solution.

信用性の判断は、信用されるべきエンティティによって満たされるべき期待に基づいている。システムの信用性の期待、その要素を含め、システムの能力、性能、セキュリティ、その他の要件に見出される。これらの判断は、信用性に関連する要件が問題を正確に反映し、解決策を正確に定義し、かつ解決策によって満たされていることが検証可能である範囲でのみ意味がある。

> The trustworthiness requirements about security derive from the protection needs, priorities, constraints, and concerns associated with the system’s ability to achieve authorized and intended behaviors and outcomes, deal with adversity, and control loss. The requirements also address the measures used to assess trustworthiness and the evidentiary data and information required to substantiate trustworthiness conclusions and grant trust. The requirements engineering discipline provides the methods, processes, techniques, and tools for this to occur.

セキュリティに関する信用性の要件は、システムが承認された意図された行動や結果を達成し、逆境に対処し、損失をコントロールする能力に関連する保護の必要性、優先順位、制約、懸念から派生している。要件はまた、信用性を評価するために使用される手段、信用性の結論を裏付け、信用を与えるために必要な証拠データと情報にも対処している。要件工学の規律は、これが発生するための方法、プロセス、技術、ツールを提供する。

> “A meaningful claim of trustworthiness cannot be based on an isolated demonstration that the system contains a protection capability assumed to be effective or sufficient. Instead, conclusions about a protection capability must have their basis on evidence that the system was properly specified, designed, and implemented with the rigor needed to deliver a system-level function in a manner deemed to be trustworthy and secure.” [2] 

「信用に値するという意味のある主張は、システムに有効または十分と仮定される保護能力が含まれているという孤立した実証に基づいてはならない。代わりに、保護能力に関する結論は、システムが信用に値すると考えられる方法でシステムレベルの機能を提供するために必要な厳格さをもって適切に指定され、設計され、実装されたことを示す証拠に基づいてなければならない。」

### F.1.2. Design Considerations / 設計上の考慮事項
> The design for a trustworthy secure system requires the application of principled engineering concepts and methods supported by evidence that provides assurance that all security-relevant claims about the system are satisfied (Section F.2).[^87] Some considerations that apply to achieving trustworthiness in system design are:

信用に値する安全なシステムの設計は、システムに関するすべてのセキュリティ関連の主張が満たされていることを保証する証拠に支えられた原則的なエンジニアリングの概念と方法の適用を要求する（セクションF.2）[^87j]。システム設計において信用性を達成するために適用されるいくつかの考慮事項は以下の通りである：

> * **Composition**<br />
  Trustworthiness judgments are compositional. They must align with how the set of composed elements provides a system capability. The way that the system is composed from its system elements must include the design principles of Compositional Trustworthiness and, to the extent practical, Structured Decomposition and Composition.

* **構成**<br />
  信用性の判断は構成的である。これらは、構成された要素の集合がシステムの能力を提供する方法と整合する必要がある。システムがそのシステム要素から構成される方法には、実用的な範囲で、構成的信用性の設計原則と、構造化された分解と構成を含める必要がある。

> * **States, Modes, and Transitions**<br />
  Ideally, the implemented system design will result in a system that continually remains in secure states and modes with secure transitions between states and modes (Section 3.2).<br />
  Realistically, the system will have insecure and indeterminant (i.e., unknown if secure or insecure) systems states and modes. The design must account for these cases and provide the capability to transition from insecure and indeterminant states and modes to secure states and modes (Protective Recovery).

* **状態、モード、および遷移**<br />
  理想的には、実装されたシステムデザインにより、システムは常に安全な状態とモードに留まり、状態とモードの間の安全な遷移が行われる（セクション3.2）。<br />
  現実的には、システムには安全でない、または不確定（つまり、安全か不安全かが不明）なシステムの状態とモードが存在する。デザインはこれらのケースを考慮し、安全でない、または不確定な状態とモードから安全な状態とモードへの遷移機能を提供する必要がある（保護的回復）。

> * **Failure Propagation**<br />
  All systems fail at some point. When a failure occurs, another failure scenario or the creation of a new failure scenario should not be triggered or invoked (Protective Failure). Designing without single points of failure (Redundancy) – including not having common mode failures (Diversity) – can help isolate system element failures while providing the required system capabilities. Additionally, the response to failure should not lead to loss or other failures (Protective Recovery).

* **故障伝播**<br />
  すべてのシステムはいずれかの時点で故障する。故障が発生した場合、他の故障シナリオの引き金となったり、新しい故障シナリオを作り出したりしてはならない（保護的故障）。単一障害点（冗長性）を持たない設計 - 共通モード故障（多様性）を含まないことも - は、必要なシステム能力を提供しながらシステム要素の故障を隔離するのに役立つ。さらに、故障への対応が損失や他の故障につながらないようにする必要がある（保護的回復）。

> * **Anomaly Detection**<br />
  Anomaly Detection provides situational awareness that allows the system to decide and recommend corrective actions to account for actual and potential deviations from accepted norms.

* **異常検出**<br />
  異常検出は、システムが実際および潜在的な受け入れられた規範からの逸脱を考慮に入れて、修正行動を決定し推奨することを可能にする状況認識を提供する。

> * **Trades**<br />
  Not every system element has trustworthiness that is sufficient for its intended purpose. A deficiency in trustworthiness can result from:<br />
  • Technical feasibility and practicality issues<br />
  • Cost and schedule issues of what is feasible and practical<br />
  • The limits of certainty (i.e., what is not known, what cannot be known, and what is underappreciated [known or could be known but dismissed prematurely])<br />
  The trade space is the rigorous application of the design principles that provide a basis for the necessary design decisions to maximize the trustworthiness of individual system elements and aggregates of elements. For example, in addressing the feasibility and practicality of cost and schedule issues, the design principle of minimizing the number of system elements that must be trusted (Minimal Trusted Elements) is applied. This reduces the size and scope of the effort and potentially reduces the expense of generating evidence of trustworthiness.

* **トレード**<br />
  すべてのシステム要素がその意図された目的に対して十分な信用性を持つわけではない。信用性の不足は次の原因で生じる可能性がある：<br />
  • 技術的実現可能性および実用性の問題<br />
  • 実現可能で実用的なもののコストおよびスケジュールの問題<br />
  • 確実性の限界（つまり、知られていないこと、知ることができないこと、及び過小評価されていること（知られているかもしれないが早計に却下されたこと））<br />
  トレード空間は、個々のシステム要素および要素の集合体の信用性を最大化するために必要な設計決定の基盤を提供する設計原則を厳格に適用することである。例えば、コストおよびスケジュールの問題の実現可能性と実用性に対処する際、信用する必要があるシステム要素の数を最小限にする（最小限の信用された要素）という設計原則が適用される。これにより、努力の規模と範囲が減少し、信用性の証拠を生成する費用が潜在的に削減される。

[^87]: > Constraints and claims are expressed in terms of functional correctness, strength of function, concerns for asset loss and consequences, and the protection capability derived from adherence to standards or from the use of specific processes, procedures, or methods.

[^87j]: 制約と主張は、機能的正確性、機能の強度、資産損失および結果に対する懸念、および基準への遵守または特定のプロセス、手順、または方法の使用から派生する保護能力の観点から表現される。

## F.2. Assurance / 保証
> Assurance is the grounds for justified confidence that a claim or set of claims has been or will be achieved [61]. Assurance is a complex and multi-dimensional property of the system that builds over time. Assurance must be planned, established, and maintained in alignment with the system throughout the system life cycle.

保証とは、ある主張または一連の主張が達成された、または達成されるという正当な確信の根拠である[61]。保証は、時間をかけて構築されるシステムの複雑で多次元的な特性である。保証は、システムのライフサイクルを通じてシステムと一致して計画され、確立され、維持されなければならない。

> Adequate security judgments should be based on the level of confidence in the ability of the system to protect itself against asset loss and the associated consequences across all forms of adversity.[^88] It cannot be based solely on individual efforts, such as demonstrating compliance, functional testing, or adversarial penetration tests. Judgments include what the system cannot do, will not do, or cannot be forced to do. These judgments of non-behavior must be grounded in sufficient confidence in the system’s ability to correctly deliver its intended function in the presence and absence of adversity and to do so when used in accordance with its design intent.

十分なセキュリティ判断は、システムがあらゆる形態の逆境に対して資産損失および関連する結果から自身を保護する能力に対する確信のレベルに基づくべきである[^88j]。それは、コンプライアンスの実証、機能テスト、または敵対的な侵入テストなどの個別の努力だけに基づくことはできない。判断には、システムが行えないこと、行わないであろうこと、または強制的に行えないことが含まれる。これらの非行動の判断は、逆境の有無にかかわらず、システムがその設計意図に従って使用された場合に、意図された機能を正確に提供する能力に十分な確信に基づいていなければならない。

> The needed evidentiary basis for such judgments derives from well-formed and comprehensive evidence-producing activities that address the requirements, design, properties, capabilities, vulnerabilities, and effectiveness of security functions. These activities include a combination of demonstration, inspection, analysis, testing, and other methods required to produce the needed evidence. The evidence acquired from these activities informs reasoning by qualified subjectmatter experts to interpret the evidence to substantiate the assurance claims made while considering other emergent properties that the system may possess.

そのような判断に必要な証拠の基盤は、要件、設計、特性、能力、脆弱性、およびセキュリティ機能の有効性に対処する、整形された包括的な証拠生成活動から派生する。これらの活動には、必要な証拠を生成するために必要な実証、検査、分析、テスト、その他の方法の組み合わせが含まれる。これらの活動から得られる証拠は、資格を持つ専門家による推論に情報を提供し、システムが持つ可能性のある他の新規特性を考慮しながら、保証の主張を裏付けるための証拠の解釈に役立つ。

[^88]: > The term adversity refers to those conditions that can cause a loss of assets (e.g., threats, attacks, vulnerabilities, hazards, disruptions, and exposures).

[-88j]: 「逆境」という用語は、資産の損失を引き起こす可能性のある条件を指す（例えば、脅威、攻撃、脆弱性、危険、中断、および露出）。

### VENEER SECURITY / うわべのセキュリティ
> Assurance is difficult but necessary.

保証は困難だが必要である。

> “I’ve covered a lot of material in this book, some of it quite tricky. But I’ve left the hardest parts to the last. First, there’s the question of assurance …“ [5].

「この本では多くの内容を扱ったが、中にはかなり厄介なものもある。しかし、最も難しい部分は最後に残した。まず、保証の問題だ…。」

> Veneer security is security functionality provided without corresponding assurance so that the functionality only appears to protect resources when it does not. Veneer security results in a false sense of security and, in fact, increases risk due to the uncertainty about the behavior and outcomes produced by the security functionality in the presence and absence of adversity. Veneer security must be avoided [62].

うわべのセキュリティとは、対応する保証なしに提供されるセキュリティ機能のことで、その機能がリソースを保護しているように見えるだけで、実際には保護していないものである。うわべのセキュリティは、誤った安心感をもたらし、実際、逆境があるときとないときのセキュリティ機能によって生じる振る舞いや結果が不確実であるために、リスクを増大させる。うわべだけのセキュリティは避けなければならない。

> Compliance is a form of “veneer security.” While compliance may have an important informing role in judgments of trustworthiness, compliance-based judgments – like other forms of veneer security – do not suffice as the sole evidentiary basis for assurance and the associated judgments of trustworthiness.

コンプライアンスは、「うわべのセキュリティ」の一形態である。コンプライアンスは、信頼性の判断において重要な情報提供の役割を果たすかもしれないが、コンプライアンスに基づく判断は、他のうわべのセキュリティの形態と同様、保証とそれに関連する信頼性の判断の唯一の証拠能力として十分ではない。

### F.2.1. Security Assurance Claims / セキュリティ保証の主張
> From a security perspective, a top-level claim addresses freedom from the conditions that cause asset loss and the associated consequences. Specifically, this means the system will adequately contribute to freedom from the conditions that cause asset loss and the associated consequences.

セキュリティの観点から、トップレベルの主張は、資産損失を引き起こす制約からの解放とそれに伴う結果からの解放に対応する。具体的には、このシステムは資産損失を引き起こす制約からの解放と、それに伴う結果からの解放に十分に貢献するであろう。

> Top-level claims decompose in a structured manner into subclaims about the desired attributes of a trustworthy secure system. Subclaims address the requirements, design, implementation, methods, and adversities that demonstrate that the system adequately contributes to ensuring only authorized and intended system behaviors and outcomes. These subclaims are derived from concerns about the completeness and accuracy of stakeholder and system requirements,[^89] enforcement of the security policy, proper implementation of the design, proper maintenance of the system, the usability of the system,[^90] and the avoidance, minimization, and mitigation of defects, errors, and vulnerabilities.[^91] Other subclaims may exist involving the ability to exhibit predictable behavior while operating in secure states in the presence and absence of adversity and the ability to recover from an insecure state. Claims can be expressed in terms of functional correctness, strength of function, and the protection capability derived from adherence to standards and/or from the use of specific processes, procedures, and methods.

トップレベルの主張は、信用に値する安全なシステムの望ましい属性に関する下位の主張へと、構造的に分解される。下位の主張は、システムが認可された意図されたシステムの振る舞いと結果を保証するために十分に貢献することを実証する要件、設計、実装、方法、および逆境に対処する。これらの下位の主張は、利害関係者およびシステム要件の完全性と正確さに関する懸念[^89]、セキュリティポリシーの適用、設計の適切な実装、システムの適切な維持、システムの使用可能性[^90]、欠陥、エラー、脆弱性の回避、最小化、および緩和[^91]から導かれる。その他の下位の主張には、逆境の存在および不在で安全な状態で動作しながら予測可能な振る舞いを示す能力や、不安全な状態から回復する能力に関与するものが存在するかもしれない。主張は、機能の正確性、機能の強度、および基準への遵守や特定のプロセス、手順、方法の使用から導かれる保護能力の観点から表現できる。

#### LEARNING FROM SAFETY / 安全からの学び
> The NASA System Safety Handbook [6] describes the relevant claims to be met in terms of the top-level claim that the system is adequately safe with subclaims, including that the system is designed to be as safe as reasonably practicable, built to be as safe as reasonably practicable, and operated as safely as reasonably practicable.

NASAのシステム安全ハンドブック[6]では、システムが十分に安全であるというトップレベルの主張に関連する主張を述べている。これには、システムが合理的に実現可能な限り安全に設計され、合理的に実現可能な限り安全に構築され、合理的に実現可能な限り安全に運用されるというサブクレームが含まれる。

[^89]: > Claims are not expressed solely as a restatement of the security functional and performance requirements. Doing so only provides assurance that the security requirements are satisfied with the implicit assumption that the requirements are correct, provide adequate coverage, and accurately reflect stakeholder needs and concerns.

[^89j]: 主張は、セキュリティ機能および性能要件の単なる再述としてのみ表現されるわけではない。そのような方法では、要件が正しいこと、十分な範囲をカバーしていること、および利害関係者のニーズと懸念を正確に反映しているという暗黙の仮定のもとで、セキュリティ要件が満たされていることの保証が提供されるだけである。

[^90]: > Most system failures have a human component. Thus, assurance must consider human frailty [5]. Operator behavior is a product of the environment (including its systems) in which it occurs [36].

[^90j]: ほとんどのシステムの失敗には人間の要素が関与している。したがって、保証は人間の弱さを考慮しなければならない[5]。オペレーターの行動は、それが発生する環境（システムを含む）の産物である[36]。

[^91]: > Not all vulnerabilities can be mitigated to an acceptable level. There are three classes of vulnerabilities in systems: (1) vulnerabilities whose existence is known and either eliminated or made to be inconsequential, (2) vulnerabilities whose existence is known but that are not sufficiently mitigated, and (3) unknown vulnerabilities that constitute an element of uncertainty. That is, the fact that the vulnerability has not been identified should not give increased confidence that the vulnerability does not exist. Determining the effect of vulnerabilities that are in the delivered system and the risk posed by those vulnerabilities and accepting uncertainty about the existence of a vulnerability that will only become known over time are important aspects that are addressed by assurance.

[^90j]: 全ての脆弱性を許容可能なレベルまで緩和することはできない。システムには三つの脆弱性のクラスがある：(1) 存在が知られており、排除されたか、無意味にされた脆弱性、(2) 存在が知られているが十分に緩和されていない脆弱性、そして (3) 不明な脆弱性で、これは不確実性の要素を構成する。つまり、脆弱性が特定されていないという事実は、その脆弱性が存在しないという確信を高めるものではない。配信されたシステム内の脆弱性の影響を判断し、それらの脆弱性によってもたらされるリスクと、時間が経つにつれてのみ知られるようになる脆弱性の存在に関する不確実性を受け入れることは、保証によって対処される重要な側面である。

### F.2.2. Approaches to Assurance / 保証へのアプローチ
> There are three general approaches to assurance. These assurance approaches can vary based on the type of evidence, how the evidence is acquired, the strength of the judgments made based on the acquired evidence, and the extent to which the assurance matches decision-making needs.

保証には、一般的に三つのアプローチが存在する。これらの保証のアプローチは、証拠の種類、証拠の取得方法、取得した証拠に基づく判断の強度、及び信頼性が意思決定のニーズにどれだけマッチしているかに応じて変わることがある。

> From weakest to strongest, the assurance approaches are axiomatic, analytic, and synthetic.

保証のアプローチを弱いものから強いものの順に並べると、公理的、分析的、統合的となる。

> * **Axiomatic Assurance** (assurance by assertion) is based on beliefs accepted on faith in an artifact or process. The beliefs are often accepted because they are not contradicted by experiment or demonstration. Axiomatic assurance is not suited to complex scenarios [62].
>   * Demonstration of conformance and compliance are types of axiomatic assurance. While useful, they are not well-suited as the sole basis of assurance for complex scenarios.

* **公理的保証**（言明による保証）は、成果物やプロセスに対する信念を信仰に基づいて受け入れることに基づいている。これらの信念は、実験や実証によって否定されないためにしばしば受け入れられる。公理的保証は複雑なシナリオには適していない。[62]
  * 適合性や遵守の実証は公理的保証のタイプである。有用ではあるが、複雑なシナリオの保証の唯一の基盤としては適していない。

> * **Analytic Assurance** (assurance by test and analysis) derives from testing or reasoning to justify conclusions about properties of interest. Belief is relocated from an artifact or process to trust in some method of analysis. The feasibility of establishing an analytic basis depends on the amount of work involved in performing the analysis and on the soundness of any assumptions underlying that analysis. Analytic methods are most relevant in a model that spans all relevant uses and all interfaces to the environment. That is, the model must not ignore too many details.
>   * Testing demonstrates the presence but not the absence of errors and vulnerabilities.
Testing and analyses will have uncertainty that cannot be ignored, especially when they lack comprehensiveness. Uncertainty contributes to risk.

* **分析的保証**（テストと分析による保証）は、興味のある特性に関する結論を正当化するためのテストや推論から派生する。信念は成果物やプロセスから分析の方法への信頼に移される。分析的基盤を確立する実現可能性は、分析を行うための作業量と、その分析に基づく仮定の健全性に依存する。分析的方法は、関連するすべての使用法と環境への全てのインターフェイスをカバーするモデルで最も関連性が高い。つまり、モデルはあまりにも多くの詳細を無視してはならない。
  * テストはエラーや脆弱性の存在を実証するが、その不存在を実証するわけではない。テストと分析には、特に包括性に欠ける場合、無視できない不確実性がある。不確実性はリスクに寄与する。

> * **Synthetic Assurance** (assurance by structured reasoning) derives from the method of composition of the “components of assurance” (i.e., the assurance derives from the manner of synthesis of the constituent parts). It requires that assurance be a consideration at every step of design and implementation, from the smallest components to the final subsystem realization.
>   * The assurance case described in [30] is an example of structured reasoning (Section 4.3).
Structured reasoning serves to fill the gaps associated with the axiomatic and analytic assurance approaches. Since synthetic assurance is based on the expert judgment of available evidence, it is not complete. However, synthetic assurance does further reduce uncertainty and, thus, reduces risk.

* **統合的保証**（構造化された推論による保証）は、「保証の要素」（すなわち、構成部分の合成方法から保証が派生する）の構成方法から派生する。これは、最小のコンポーネントから最終的なサブシステムの実現に至るまで、設計と実装の各段階で保証を考慮することを要求する。
  * [30]に記述されている保証ケースは、構造化された推論の例である（セクション4.3）。構造化された推論は、公理的および分析的保証アプローチに関連するギャップを埋めるために役立つ。統合的保証は利用可能な証拠に基づく専門家の判断に基づいているため、完全ではない。しかし、統合的保証は不確実性をさらに減少させ、それによってリスクを減少させる。

Assurance depends on the quality of the evidence used in arguments demonstrating that claims about the system are satisfied. Assurance evidence can be obtained either directly through measurement, testing, observation, or inspection or indirectly through analysis, including the analysis of data obtained from measurement, testing, observation, or inspection. Evidence must have sufficient quality in accuracy, credibility, relevance, rigor, and quantity. The accuracy, credibility, and relevance of evidence should be confirmed prior to its use. For example, some evidence can support arguments for strength of function, others for negative requirements (i.e., what will not happen), and still other evidence for qualitative properties.

統合的保証は、システムに関する主張が満たされていることを実証する議論で使用される証拠の品質に依存する。統合的保証の証拠は、直接的に測定、テスト、観察、検査を通じて、または間接的に分析を通じて、測定、テスト、観察、検査から得られたデータの分析を含む方法で得ることができる。証拠は、正確性、信頼性、関連性、厳密さ、量の点で十分な品質を持つ必要がある。証拠の正確性、信頼性、関連性は、使用する前に確認されるべきである。例えば、ある証拠は機能の強度に関する主張を支持することができ、他の証拠は否定的な要件（すなわち、起こらないこと）に対して、また別の証拠は質的特性に対して支持することができる。

#### ASSURANCE CASE / 保証ケース
> An assurance case is a reasoned, auditable artifact that is created to support the contention that a top-level claim is satisfied. The assurance case includes systematic argumentation, evidence, and explicit assumptions that support the claim.

保証ケースは、上位レベルの主張が満たされているという論争を支持するために作成される、合理的で監査可能な成果物である。保証ケースには、主張を支持するための体系的な論証、証拠、そして明示的な前提が含まれている。

> An assurance case contains the following elements [30]:
> * One or more claims about properties
> * Arguments that logically link the evidence and any assumptions
> * A body of evidence
> * Justification of the choice of a top-level claim and the method of reasoning

保証ケースには以下の要素が含まれる[30]：
* 特性に関する一つ以上の主張
* 証拠と任意の前提を論理的に結びつける論証
* 証拠の本体
* 上位レベルの主張の選択と推論方法の正当化

> Assurance cases have numerous advantages over other means for obtaining confidence, such as in the areas of comprehension, informing needed allocation responsibilities, information organization, and robust due diligence [63]. These advantages were greater in areas with otherwise insufficient methods for achieving high assurance. Additionally, assurance cases were determined to be more efficient for complex and novel systems, as well as systems in need of high assurance.

保証ケースは、理解、必要な責任分担の情報提供、情報の整理、および厳格な適切な注意[63]の領域など、確信を得るための他の手段よりも多くの利点がある。これらの利点は、高度な保証を達成するための方法が不十分な領域でより大きかった。さらに、保証ケースは、複雑で革新的なシステムや、高度な保証が必要なシステムに対してより効率的であると判断された。

> Many formalizations and tools for building assurance cases have been developed in recent years, including the Goal Structuring Notation (GSN) [64] and NASA’s AdvoCATE: Assurance Case Automation Toolset [65].

近年、保証ケースを構築するための多くの形式化手法とツールが開発されている。これには、ゴール構造化表記（GSN）[64]やNASAのAdvoCATE：保証ケース自動化ツールセット[65]が含まれる。

### F.2.3. Assurance Needs
> Assurance is a need that is to be engineered and satisfied similar to the need to engineer the system capability to satisfy specified capability needs. Assurance needs for trustworthy secure systems are grounded in the concerns of loss and adverse effects due to intentional and unintentional adversity (Commensurate Trustworthiness, Substantiated Trustworthiness, Commensurate Rigor). Assurance needs include the evidence-basis for reasoning, the degree of rigor to acquire and interpret the evidence, and the selection of the methods, tools, and processes used throughout the system life cycle. Similar to capability and performance needs, assurance needs, expectations, priorities, and constraints should be expressed as system requirements and achieved, tracked, and maintained within the systems engineering effort.

保証は、指定された能力ニーズを満たすためのシステム能力をエンジニアリングする必要性と同様に、エンジニアリングされ、満たされるべきニーズである。信用に値するセキュアなシステムのための保証ニーズは、意図的および非意図的な逆境による損失と悪影響の懸念に基づいている（相応の信用性、裏付けられた信用性、相応の厳密さ）。保証ニーズには、推論のための証拠基盤、証拠を取得し解釈するための厳密さの度合い、およびシステムのライフサイクルを通じて使用される方法、ツール、プロセスの選択が含まれる。能力およびパフォーマンスのニーズと同様に、保証ニーズ、期待、優先順位、制約はシステム要件として表現され、システムズ エンジニアリングの努力の中で達成され、追跡され、維持されるべきである。

> Assurance needs determine the type of evidence and the rigor associated with the activities, methods, and tools used to acquire the evidence to satisfy the following cases:
> * *What is to be accomplished in the systems engineering effort*: The realization of the design for a secure system
> * *The means to conduct the systems engineering effort*: The methods, processes, and tools employed (driven by rigor and assurance objectives) to realize the design for a secure system
> * *The results of the systems engineering effort*: The substantiated effectiveness of the realized design of the secure system

保証ニーズは、以下のケースを満たすために証拠を取得する活動、方法、およびツールに関連する証拠の種類と厳密さを決定する：
* *システムズ エンジニアリングの努力で達成すべきこと*：セキュアなシステムのための設計の実現
* *システムズ エンジニアリングの努力を行う手段*：セキュアなシステムの設計を実現するために用いられる方法、プロセス、およびツール（厳密さと保証の目的によって推進される）
* *システムズ エンジニアリングの努力の結果*：セキュアなシステムの実現された設計の裏付けられた効果性

#### CONFIDENCE MAY BE NEGATIVE / 確信は否定的である可能性がある
> Assurance evidence can support a conclusion that a stated claim is not achieved or that there is an insufficient basis to conclude that the claim is supported or not supported. In either case, the assurance is negative relative to the goal of substantiating the claim. That is, the system or some part of the system is not sufficiently trustworthy and should not be trusted relative to its specified function without further action.

保証の証拠は、特定の主張が達成されていない、または主張が支持されているかどうかを結論付けるための十分な根拠がないという結論を支持することができる。いずれの場合も、保証は主張の裏付けという目標に対して否定的である。すなわち、システムまたはシステムの一部が十分に信用に値しないのであり、指定された機能に関してさらなる行動なしに信用されるべきではない。

> Assurance needs can vary and constitute a trade space that must be managed similar to how capability and performance needs can vary. The degree of rigor is the primary means of varying assurance. As shown in Figure 17, a direct relationship exists between the degree of rigor and assurance and the stakeholder’s assessment of the effects of asset loss. The assurance trade space includes the following considerations:
> * Cost, schedule, and performance
> * Architecture and design decisions
> * Selection of technology and solutions
> * Selection and employment of methods and tools
> * Qualifications necessary for subject-matter experts

保証ニーズは変動する可能性があり、能力やパフォーマンスのニーズが変動するのと同様に管理されるべきトレードの空間を構成する。厳密さの程度は、保証を変動させる主要な手段である。図17に示されているように、厳密さと保証の程度と、利害関係者による資産損失の影響の評価との間には直接的な関係が存在する。保証のトレード空間には、以下の考慮事項が含まれる：
* コスト、スケジュール、およびパフォーマンス
* アーキテクチャおよび設計の決定
* 技術およびソリューションの選択
* 方法およびツールの選択と使用
* 主題専門家に必要な資格条件

> Requirements analysis across stakeholder and system requirements determines the threshold degree of rigor that is required. When a system cannot practicably meet the needed degrees of rigor, stakeholders should have a means to determine if they will accept the associated risk.

利害関係者およびシステム要件を通じた要件分析は、必要とされる厳密さの閾値の程度を決定する。システムが実際に必要な厳密さの程度を満たすことができない場合、利害関係者は関連するリスクを受け入れるかどうかを判断する手段を持つべきである。

![Fig. 17. Assurance and Degree of Rigor in Realizing a Capability Need](fig17.png)

Fig. 17. Assurance and Degree of Rigor in Realizing a Capability Need

> The highest levels of rigor across systems can require formal methods – techniques that model systems as mathematical entities to enable rigorous verification of the system’s properties through mathematical proofs. Formal methods depend on formal specifications (i.e., statements in a language whose vocabulary, syntax, and semantics are formally defined) and a variety of models, including a formal security policy model (i.e., a mathematically rigorous specification of a system’s security policy [Appendix C]).

システム全体で最高レベルの厳密さを求める場合、公式な方法が必要となることがある。これはシステムを数学的な実体としてモデル化し、数学的な証明を通じてシステムの特性を厳格に検証する技術である。公式な方法は、公式仕様（すなわち、語彙、構文、意味論が形式的に定義された言語での声明）と、公式セキュリティポリシーモデル（すなわち、システムのセキュリティポリシーの数学的に厳格な仕様\[[付録C](Appendex-C.md)]）を含む様々なモデルに依存する。

> Due to associated costs and complexity, formal methods are typically limited to engineering efforts where only the highest levels of assurance are needed, such as the formal modeling, specification, and verification of security policy and the implementation that enforces the policy (Section D.4.2). In this case, the security policy model is verified as complete for its scope of control and as self-consistent. The verified security policy model then serves as a foundation to verify the models of the design and implementation of the mechanisms that provide for decisionmaking and the enforcement of those decisions.

関連するコストと複雑さのため、公式な方法は通常、最高レベルの保証が必要なエンジニアリング努力に限定される。例えば、セキュリティポリシーの公式モデリング、仕様、および検証、そしてそのポリシーを施行する実装（セクションD.4.2）。この場合、セキュリティポリシーモデルは、その管理範囲において完全であり、自己一貫性があるとして検証される。検証されたセキュリティポリシーモデルは、意思決定を行い、それらの決定を施行するためのメカニズムの設計と実装のモデルを検証するための基盤として機能する。