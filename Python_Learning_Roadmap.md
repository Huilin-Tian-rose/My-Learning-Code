# Python 数据分析与科学计算学习路线图

**个人:** 田荟琳  
**专业:** 数据科学  
**目标:** 系统掌握Python数据分析全栈技能，为参与科研项目与学科竞赛打下坚实基础。  
**起始日期:** 2025年9月24日  
**更新日志:** 本计划将根据学习进度动态调整。

## 学习理念
 **项目驱动:** 每个阶段均以小型实战项目巩固知识。
 **持续记录:** 代码、笔记、问题均通过GitHub进行版本管理。

## 第一阶段：编程基础与核心语法 (预计: 3周)
**目标:** 掌握Python编程的基本逻辑。
- [x] 基础语法：变量、数据类型、运算符、基本输出
- [x] 数据结构：列表、元组、字典
- [x] 流程控制：条件语句、for循环的基础操作与复杂运用，条件循环语句、while循环，跳出循环的办法，循环的综合应用（嵌套循环、遍历整数列表）
- [ ] 函数与模块：自定义函数、使用内置模块
## 详细内容
 1. **编程中的"文本"** - 字符串操作和注释
2. **变量与赋值** - 变量定义和数据存储
3. **编程中的"数字"** - 数值运算和格式化
4. **编程中的"真"与"假"** - 布尔逻辑和条件判断
5. **单向选择的判断** - if语句和条件执行
6. **双向选择的判断** - if-else语句和分支选择
## 代码练习的大致内容
def string_demo():
    """No.001 浮世三千，吾爱有三 - 字符串基础"""
    text = "浮世三千，吾爱有三"
    print("原始文本:", text)
    print("文本长度:", len(text))
    print("前三个字:", text[:3])
    return text

def comment_practice():
    """No.002 注释练习 - 代码注释说明"""
    # 这是单行注释
    name = "Python学习者"
    
    """
    这是多行注释
    可以写更详细的说明
    """
    age = 20
    
    print(f"姓名: {name}, 年龄: {age}")
    return name, age

def string_methods():
    """字符串常用方法练习"""
    text = "  Hello, Python!  "
    
    # 去除空格
    cleaned = text.strip()
    print(f"去除空格: '{cleaned}'")
    
    # 大小写转换
    print(f"大写: {text.upper()}")
    print(f"小写: {text.lower()}")
    
    # 字符串替换
    replaced = text.replace("Python", "World")
    print(f"替换后: {replaced}")
    
    return cleaned

if __name__ == "__main__":
    string_demo()
    comment_practice()
    string_methods()

def weight_loss_record():
    """No.003 减肥记录 - 变量赋值练习"""
    initial_weight = 75.5  # 初始体重
    current_weight = 72.3  # 当前体重
    weight_loss = initial_weight - current_weight
    
    print("=== 减肥记录 ===")
    print(f"初始体重: {initial_weight}kg")
    print(f"当前体重: {current_weight}kg")
    print(f"已减体重: {weight_loss:.1f}kg")
    
    return weight_loss

def internet_cafe():
    """No.004 夜曲网吧 - 多变量操作"""
    hours = 3
    rate = 5  # 每小时5元
    total_cost = hours * rate
    
    print(f"上网时间: {hours}小时")
    print(f"每小时费率: {rate}元")
    print(f"总费用: {total_cost}元")
    
    return total_cost


def mountain_temple():
    """No.006 夜宿山寺 - 字符串变量操作"""
    poet = "李白"
    poem_title = "夜宿山寺"
    poem_line1 = "危楼高百尺"
    poem_line2 = "手可摘星辰"
    
    full_poem = f"""
    《{poem_title}》 - {poet}
    
    {poem_line1}，
    {poem_line2}。
    """
    
    print(full_poem)
    return full_poem

if __name__ == "__main__":
    weight_loss_record()
    internet_cafe()
    format_output()
    mountain_temple()

    def calculate_bmi():
    """No.007 BMI身体质量指数"""
    weight = 70  # 公斤
    height = 1.75  # 米
    
    bmi = weight / (height ** 2)
    
    print("=== BMI计算 ===")
    print(f"体重: {weight}kg")
    print(f"身高: {height}m")
    print(f"BMI指数: {bmi:.2f}")
    
    # BMI分类
    if bmi < 18.5:
        category = "偏瘦"
    elif bmi < 24:
        category = "正常"
    elif bmi < 28:
        category = "偏胖"
    else:
        category = "肥胖"
    
    print(f"体型分类: {category}")
    return bmi, category


def english_number_format():
    """No.009 英语数字格式 - 数字格式化"""
    number = 1234567.8912
    
    formats = {
        "整数": f"{number:,.0f}",
        "两位小数": f"{number:,.2f}",
        "科学计数法": f"{number:.2e}",
        "百分数": f"{0.4567:.1%}",
        "前导零": f"{42:05d}"
    }
    
    print("=== 数字格式化示例 ===")
    for desc, formatted in formats.items():
        print(f"{desc}: {formatted}")
    
    return formats

def midautumn_sentiment():
    """No.010 情感中秋 - 数学运算应用"""
    # 中秋相关数据
    mooncake_price = 25.8
    family_members = 6
    budget = 200
    
    max_mooncakes = budget // mooncake_price  # 整除
    change = budget % mooncake_price  # 取余
    
    print("=== 中秋情感计算 ===")
    print(f"月饼单价: {mooncake_price}元")
    print(f"家庭成员: {family_members}人")
    print(f"预算金额: {budget}元")
    print(f"最多可买月饼: {int(max_mooncakes)}个")
    print(f"剩余金额: {change:.1f}元")
    print(f"人均可享: {max_mooncakes / family_members:.1f}个月饼")
    
    return max_mooncakes, change

if __name__ == "__main__":
    calculate_bmi()
    breakfast_calculation()
    english_number_format()
    midautumn_sentiment()

def judge_fallacy():
    """No.011 判断谬误 - 布尔值基础"""
    # 基本布尔值
    true_value = True
    false_value = False
    
    print("=== 布尔值基础 ===")
    print(f"True的值: {true_value}")
    print(f"False的值: {false_value}")
    
    # 比较运算
    a, b = 10, 5
    comparisons = {
        "等于": a == b,
        "不等于": a != b,
        "大于": a > b,
        "小于": a < b,
        "大于等于": a >= b,
        "小于等于": a <= b
    }
    
    print("\n=== 比较运算 ===")
    for operation, result in comparisons.items():
        print(f"10 {operation} 5: {result}")
    
    return comparisons

def target_weight():
    """No.012 目标体重 - 布尔逻辑应用"""
    current_weight = 68.5
    target_min = 65.0
    target_max = 70.0
    
    # 布尔判断
    within_target = target_min <= current_weight <= target_max
    under_weight = current_weight < target_min
    over_weight = current_weight > target_max
    
    print("=== 目标体重判断 ===")
    print(f"当前体重: {current_weight}kg")
    print(f"目标范围: {target_min}-{target_max}kg")
    print(f"是否在目标范围内: {within_target}")
    print(f"是否偏轻: {under_weight}")
    print(f"是否偏重: {over_weight}")
    
    # 逻辑运算
    healthy_bmi = True
    regular_exercise = True
    
    healthy_lifestyle = healthy_bmi and regular_exercise
    need_improvement = not healthy_lifestyle
    
    print(f"健康生活方式: {healthy_lifestyle}")
    print(f"需要改进: {need_improvement}")
    
    return within_target, healthy_lifestyle

def player_selection():
    """No.013 小球员的选拔 - 复杂布尔逻辑"""
    age = 12
    height = 155  # 厘米
    skill_level = "良好"
    
    # 选拔条件
    age_qualified = 10 <= age <= 14
    height_qualified = height >= 150
    skill_qualified = skill_level in ["良好", "优秀"]
    
    # 综合判断
    qualified = age_qualified and height_qualified and skill_qualified
    
    print("=== 球员选拔系统 ===")
    print(f"年龄: {age}岁 - 合格: {age_qualified}")
    print(f"身高: {height}cm - 合格: {height_qualified}")
    print(f"技能: {skill_level} - 合格: {skill_qualified}")
    print(f"最终选拔结果: {'通过' if qualified else '不通过'}")
    
    # 详细判断
    if not age_qualified:
        print("原因: 年龄不符合要求")
    if not height_qualified:
        print("原因: 身高不符合要求")
    if not skill_qualified:
        print("原因: 技能水平不足")
    
    return qualified

if __name__ == "__main__":
    judge_fallacy()
    target_weight()
    player_selection()
def right_triangle():
    """No.014 直角三角形判断"""
    a, b, c = 3, 4, 5
    
    # 检查是否为直角三角形
    sides = [a, b, c]
    sides.sort()  # 排序，c为最大边
    
    is_right_triangle = sides[0]**2 + sides[1]**2 == sides[2]**2
    
    print("=== 直角三角形判断 ===")
    print(f"三角形边长: {a}, {b}, {c}")
    
    if is_right_triangle:
        print("这是一个直角三角形")
        # 计算面积
        area = (sides[0] * sides[1]) / 2
        print(f"直角边: {sides[0]}和{sides[1]}")
        print(f"面积: {area}")
    else:
        print("这不是一个直角三角形")
    
    return is_right_triangle

def bmi_2_0():
    """No.015 BMI指数2.0 - 条件判断进阶"""
    weight = float(input("请输入体重(kg): "))
    height = float(input("请输入身高(m): "))
    
    bmi = weight / (height ** 2)
    
    print(f"\n您的BMI指数: {bmi:.2f}")
    
    # 详细分类判断
    if bmi < 18.5:
        category = "体重过轻"
        suggestion = "建议增加营养，适当增重"
    elif bmi < 24:
        category = "正常体重"
        suggestion = "保持良好生活习惯"
    elif bmi < 28:
        category = "超重"
        suggestion = "建议适当运动，控制饮食"
    else:
        category = "肥胖"
        suggestion = "建议咨询医生，制定减肥计划"
    
    print(f"体型分类: {category}")
    print(f"健康建议: {suggestion}")
    
    return bmi, category

def choose_phone():
    """No.016 选择一款手机 - 多条件判断"""
    budget = float(input("请输入预算(元): "))
    preference = input("偏好类型(游戏/拍照/日常): ")
    
    print("\n=== 推荐手机 ===")
    
    if budget >= 5000:
        if preference == "游戏":
            recommendation = "推荐: 游戏手机ROG/黑鲨，性能强劲"
        elif preference == "拍照":
            recommendation = "推荐: 华为P系列/小米Ultra，拍照出色"
        else:
            recommendation = "推荐: iPhone/三星S系列，综合体验好"
    
    elif budget >= 3000:
        if preference == "游戏":
            recommendation = "推荐: 红魔/realme GT，性价比游戏手机"
        elif preference == "拍照":
            recommendation = "推荐: 小米/荣耀数字系列，拍照不错"
        else:
            recommendation = "推荐: 小米/OPPO中端系列，均衡实用"
    
    else:
        recommendation = "推荐: 红米/realme Q系列，入门性价比选择"
    
    print(recommendation)
    return recommendation

def compare_area():
    """No.017 比较面积"""
    import math
    
    # 不同形状的面积
    square_side = 5
    circle_radius = 3
    rectangle_length, rectangle_width = 6, 4
    
    areas = {
        "正方形": square_side ** 2,
        "圆形": math.pi * circle_radius ** 2,
        "长方形": rectangle_length * rectangle_width
    }
    
    print("=== 面积比较 ===")
    for shape, area in areas.items():
        print(f"{shape}面积: {area:.2f}")
    
  

def simplify_with_else():
    """No.018 使用else简化代码"""
    number = int(input("请输入一个数字: "))
    
    # 传统写法
    if number % 2 == 0:
        result = "偶数"
    else:
        result = "奇数"
    
    print(f"{number}是{result}")
    
    # 简化后的判断
    age = 18
    status = "成年人" if age >= 18 else "未成年人"
    print(f"年龄{age}岁: {status}")
    
    return result

def calculate_shipping():
    """No.019 计算运费"""
    weight = float(input("请输入包裹重量(kg): "))
    distance = int(input("请输入运输距离(km): "))
    
    # 基础运费
    base_rate = 10
    
    # 重量附加费
    if weight > 5:
        weight_surcharge = (weight - 5) * 2
    else:
        weight_surcharge = 0
 

def user_login():
    """No.020 用户登录系统"""
    correct_username = "admin"
    correct_password = "123456"
    
    username = input("用户名: ")
    password = input("密码: ")
    
    print("\n=== 登录结果 ===")
    if username == correct_username and password == correct_password:
        print("登录成功！欢迎回来！")
        # 登录后的操作
        user_role = "管理员" if username == "admin" else "普通用户"
        print(f"用户角色: {user_role}")
        success = True
    else:
        print("登录失败！用户名或密码错误！")
        # 失败处理
        if username != correct_username:
            print("错误: 用户名不存在")
        else:
            print("错误: 密码不正确")
        success = False
    
    return success

def pilot_application():
    """No.021 报考飞行员"""
    print("=== 飞行员报考条件检查 ===")
    
    age = int(input("年龄: "))
    height = float(input("身高(cm): "))
    vision = float(input("视力: "))
    education = input("学历(高中/本科/硕士): ")
    
    # 条件检查
    age_ok = 18 <= age <= 25
    height_ok = 165 <= height <= 185
    vision_ok = vision >= 1.0
    education_ok = education in ["高中", "本科", "硕士"]
    
    # 综合判断
    if age_ok and height_ok and vision_ok and education_ok:
        print("\n🎉 恭喜！符合报考条件！")
        print("可以参加下一轮体检和面试")
        
    
    return qualified

if __name__ == "__main__":
    simplify_with_else()
    calculate_shipping()
    user_login()
    pilot_application()

    
**实战项目:** 
- [ ] 开发个人学习打卡器
- [ ] 编写通讯录管理程序

## 第二阶段：数据分析核心库 (预计: 4周)
**目标:** 掌握数据处理与分析的核心工具链。
- [ ] **NumPy:** 数组操作、数学运算
- [ ] **Pandas:** 数据清洗、转换、分析
- [ ] 描述性统计分析

## 第三阶段：数据可视化 (预计: 3周)
**目标:** 能够将数据转化为直观的图表。
- [ ] **Matplotlib:** 基础绘图、图表美化
- [ ] **Seaborn:** 统计图形绘制
- [ ] 可视化思维训练

## 第四阶段：数据获取与存储 (预计: 3周)
**目标:** 掌握从外部获取数据的能力。
- [ ] **SQL基础:** 查询、聚合、多表连接
- [ ] Python与数据库交互
- [ ] API接口数据获取

## 进度追踪
| 阶段 | 计划开始日期 | 状态 | 完成度 |
|------|-------------|------|--------|
| 第一阶段 | 2025- 9-24 | 实行的第三周内  | 90% |
| 第二阶段 | 2025-10-15 | 待开始 | 0% |
