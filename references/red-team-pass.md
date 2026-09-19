# Red Team Pass

Adversarial review of the leading option. Method lineage: red-teaming as structured challenge to plans and assessments (Hoffman 2017; Zenko 2015; UK MoD Red Teaming Handbook 3rd ed. 2021; CIA Tradecraft Primer 2009 — exact citations in `anchors-and-sources.md`).

## Protocol

1. **Steelman first（必做，先立后破）**：用最强形式陈述支持该选项的理由——比 brief 里写的更强。攻击一个弱化版对手不产生信息（稻草人红队在 rubric 对立面强度维度记 0）。

2. **Four attack lines**（每条至少认真试一次）：
   - **攻证据**：哪些载重 F2 从未核实？什么证据一旦出现就直接推翻关键主张（falsification test）？
   - **攻框架**：这是不是正确的问题？（「选 A 还是 B」可能真问题是「为什么必须二选一」「为什么是现在」）
   - **攻激励**：谁从这个选择中获益？信息输入是否被获益方塑形（中介、销售、急于结案的自己）？
   - **攻时机**：等待的真实成本是多少？「机不可失」有多少是卖方叙事？

3. **Survivor selection**：留下 2-3 条**修订后仍然成立**的最强反对意见。每条附一句：「如果 ___ 为真，这条反对就足以否决整个决策。」

4. **Into the memo**：幸存反对意见原样写进决策备忘录——不允许被 revision 打磨掉。复盘时它们是最有价值的对照物。

## Output format

```markdown
## Red Team（选项 X）
**Steelman**：（该选项的最强论证，2-4 句）
| # | 攻击线 | 反对意见 | 修订后是否仍成立 | 否决条件（如果___为真则足以否决） |
|---|---|---|---|---|
```

## Anti-patterns

- 红队产出全被「解释掉」——一个健康的红队 pass 应该至少改变 brief 的一处概率、证据要求或止损位；全身而退的 brief 要么极其扎实，要么红队没用力，说明是哪种。
- 用红队表演审慎（列 10 条弱反对刷数量）。3 条能否决的 > 10 条挠痒的。
- 红队之后偷偷加固 steelman——幸存反对意见带否决条件入备忘录，不做二次辩护。
