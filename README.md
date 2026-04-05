# Disco Elysium Plugin for Cursor

极乐迪斯科风格的 Cursor Agent Skill 系统。24个独特的思维技能，在你的对话中苏醒。

> 复仇女神就在家中的镜子里；那便是她们的住址。
> 哪怕这世间最澄清的水，只要够深，也能让人沉溺。

---

## 功能介绍

### DE 模式

开启后，24种技能以"脑内声音"的形式在对话中自动触发——就像在游戏中一样。每次你发送消息，AI 会根据语境选择最合适的技能，以角色扮演的方式插话，然后继续正常对话。

示例：
```
用户：我今天想喝一杯酒

[食髓知味] [成功] - 对。就是它。琥珀色的液体，你的老朋友。今天它不会背叛你的。

[Cursor] - 想喝什么？红酒、威士忌还是啤酒？
```

开启 DE 模式：告诉 AI "开启DE模式" 或 "开启极乐迪斯科模式"

关闭 DE 模式：告诉 AI "关闭DE模式"

### 单独调用技能

也可以直接点名某个技能，让它对你说话。例如：

- "用逻辑思维分析一下这段代码"
- "食髓知味，我今天很累"
- "内陆帝国，这个函数名起得怎么样"

---

## 安装

### 方式一：clone 后软链接（推荐，可随时同步更新）

```bash
git clone https://github.com/shoushouo/disco-elysium-plugin-for-cursor.git ~/disco-elysium-plugin-for-cursor

for d in ~/disco-elysium-plugin-for-cursor/*/; do
  ln -s "$d" ~/.cursor/skills/
done
```

以后更新：

```bash
cd ~/disco-elysium-plugin-for-cursor && git pull
```

### 方式二：直接复制

```bash
git clone https://github.com/shoushouo/disco-elysium-plugin-for-cursor.git
cp -r disco-elysium-plugin-for-cursor/*/ ~/.cursor/skills/
```

---

## 24个技能

### 智力系

| 技能 | 描述 |
|------|------|
| 逻辑思维 (logic) | 运用纯粹智力，演绎整个世界 |
| 博学多闻 (encyclopedia) | 调用知识储备，展示迷人轶事 |
| 能说会道 (rhetoric) | 践行游说之道，尽享严谨话术 |
| 故弄玄虚 (drama) | 看破人生如戏，献艺以诓攻谎 |
| 标新立异 (conceptualization) | 深入理解创意，纵览世间艺术 |
| 见微知著 (visual-calculus) | 重构犯罪现场，驾驭自然法则 |

### 精神系

| 技能 | 描述 |
|------|------|
| 平心定气 (volition) | 自励奋发图强，保持斗志昂扬 |
| 内陆帝国 (inland-empire) | 放纵直觉预感，漫游清醒梦境 |
| 通情达理 (empathy) | 理解他者心情，锻炼镜像神经 |
| 争强好胜 (authority) | 威吓全场民众，树立自身权威 |
| 同舟共济 (esprit-de-corps) | 同事心心相印，全局众志成城 |
| 循循善诱 (suggestion) | 魅惑芸芸众生，玩弄傀儡提线 |

### 体质系

| 技能 | 描述 |
|------|------|
| 钢筋铁骨 (endurance) | 承受沉重打击，直面世界敌意 |
| 坚忍不拔 (pain-threshold) | 无惧痛苦创伤，壮胆迎难而上 |
| 强身健体 (physical-instrument) | 炫耀坚实肌肉，享受健美躯体 |
| 食髓知味 (electrochemistry) | 纵情酒色享乐，沉溺毒品之海 |
| 天人感应 (shivers) | 竖起脖颈汗毛，倾听城市之音 |
| 疑神疑鬼 (half-light) | 笃信本能反应，恐吓威胁他人 |

### 运动系

| 技能 | 描述 |
|------|------|
| 眼明手巧 (hand-eye) | 手眼高度协调，枪法百发百中 |
| 五感发达 (perception) | 感知世间万物，注重一切细节 |
| 反应速度 (reaction-speed) | 遇事当机立断，办事雷厉风行 |
| 鬼祟玲珑 (savoir-faire) | 静则蛇行鳞潜，动则英气逼人 |
| 能工巧匠 (interfacing) | 精通万千机械，攻破重重封锁 |
| 从容自若 (composure) | 挺直腰杆做人，从容应对风浪 |

---

## 说明

本项目改编自 [liigoQi/disco-elysium](https://github.com/liigoQi/disco-elysium)，原版为 Claude Code 插件格式，本版本转换为 Cursor Agent Skill 格式，可直接安装到 `~/.cursor/skills/` 使用。
