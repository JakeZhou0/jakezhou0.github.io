---
工作满意度: "9.5"
个人成就感: "2"
心理健康: "7.1"
人际交往能力: "7.7"
职业素养: "8.9"
领导力与影响力: "4.2"
创新能力: "6.1"
身心健康自评: "7.2"
生活质量评价: "4.9"
个人成长与发展: "3.1"
---

#📦/模板

满分 10 分

```dataviewjs
const page = dv.current()

let frontmatter = page.file.frontmatter;
const scoreNameList = []
const scoreList = [];

// 遍历frontmatter对象并将键名与值分别添加到相应的列表中
for (let key in frontmatter) {
    scoreNameList.push(key);
    scoreList.push(frontmatter[key]);
}


const target = [1, 2, 3, 4, 5, 6, 7, 8, 9,10]

const option = {

  title: {

    text: "健康指标图",

  },

  tooltip: {},

  legend: {

    data: ["目标分数", "实际分数"],

  },

  radar: {

    // shape: 'circle',

    indicator: [

      { name: "工作满意度", max: 10 },

      { name: "个人成就感", max: 10 },

      { name: "心理健康", max: 10 },

      { name: "人际交往能力", max: 10 },

      { name: "职业素养", max: 10 },

      { name: "领导力与影响力", max: 10 },

      { name: "创新能力", max: 10 },
      
      { name: "身心健康自评", max: 10 },
      
      { name: "生活质量评价", max: 10 },
      
      { name: "个人成长与发展", max: 10 },

    ],

  },

  series: [

    {

      name: "目标 vs 实际",

      type: "radar",

      // areaStyle: {normal: {}},

      data: [

        {

          value: target,

          name: "目标分数",

        },

        {

          value: scoreList,

          name: "实际分数",

        },

      ],

    },

  ],

};

app.plugins.plugins['obsidian-echarts'].render(option, this.container)
```

1. **(scoreName:: 工作满意度)**：
   - 工作内容满意度: 个人对其工作任务性质、挑战性和创新性的主观评价。
   - 工作环境满意度: 对办公环境、同事关系、组织文化等的主观感受。

2. **(scoreName:: 个人成就感)**：
   - 成就动机：个体追求目标、实现任务的内在驱动力及达成后的满足感。
   - 自我效能感：对自己能够成功执行所需任务的信心程度。

3. **(scoreName:: 心理健康)**：
   - 心理压力水平：个体感受到的工作或生活压力大小。
   - 情绪稳定性：个体的情绪波动程度，是否有持久的乐观心态或容易受负面情绪困扰。

4. **(scoreName:: 人际交往能力)**：
   - 社交技巧：与他人有效沟通、建立和维护关系的能力。
   - 团队协作能力：在团队中的互动表现、贡献度和影响力。

5. **(scoreName:: 职业素养)**：
   - 职业道德与诚信：遵守职业道德规范的程度和在工作中表现出的诚实可靠程度。
   - 组织承诺：对所在组织忠诚度、归属感及愿意为其长期服务的意愿。

6. **(scoreName:: 领导力与影响力)**：
   - 建立信任：领导者在团队中赢得信赖的能力。
   - 决策影响力：个人在团队决策过程中的作用和建议被采纳的情况。

7. **(scoreName:: 创新能力)**：
   - 创意思维：发现新思路、解决问题的独特视角和方法。
   - 实践创新：将新的想法转化为实际行动和成果的表现。

8. **(scoreName:: 身心健康自评)**：
   - 身体健康状况自评：个体对自身身体状况的主观评价。
   - 精神健康自评：对自己的心理适应能力、抗压能力以及是否存在心理障碍的自我感知。

9. **(scoreName:: 生活质量评价)**：
   - 工作与生活平衡：个人在工作与私人生活之间分配时间和精力的满意度。
   - 生活幸福感：对个人生活总体满足感和幸福感的主观打分。

10. **(scoreName:: 个人成长与发展)**：
	- 学习能力与进步：个人在技能提升、知识增长方面的自我评价。
	- 职业规划清晰度：对未来职业路径的明确程度和为此所做的努力与准备。