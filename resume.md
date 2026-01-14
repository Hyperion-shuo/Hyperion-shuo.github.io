\documentclass[10pt, letterpaper]{article}

% 页面布局设置
\usepackage[
    ignoreheadfoot, 
    top=2 cm, 
    bottom=2 cm, 
    left=2 cm, 
    right=2 cm, 
    footskip=1.0 cm, 
]{geometry} 

% ==================================================
% 中文支持配置 (必须使用 XeLaTeX 编译器)
% fontset=ubuntu 使用 Overleaf 服务器自带的开源中文字体
% ==================================================
\usepackage[UTF8, fontset=ubuntu]{ctex} 

\usepackage{titlesec} 
\usepackage{tabularx} 
\usepackage{array} 
\usepackage[dvipsnames]{xcolor} 
\definecolor{primaryColor}{RGB}{0, 0, 0} 
\usepackage{enumitem} 
\usepackage{fontawesome5} 
\usepackage{amsmath} 
\usepackage[
    pdftitle={沈硕的简历},
    pdfauthor={沈硕},
    colorlinks=true,
    urlcolor=primaryColor
]{hyperref} 
\usepackage[pscoord]{eso-pic} 
\usepackage{calc} 
\usepackage{bookmark} 
\usepackage{lastpage} 
\usepackage{changepage} 
\usepackage{paracol} 
\usepackage{ifthen} 
\usepackage{needspace} 
\usepackage{iftex} 

% 移除不兼容的英文字体包
% \usepackage{charter} 

% 基础设置
\raggedright
\AtBeginEnvironment{adjustwidth}{\partopsep0pt} 
\pagestyle{empty} 
\setcounter{secnumdepth}{0} 
\setlength{\parindent}{0pt} 
\setlength{\topskip}{0pt} 
\setlength{\columnsep}{0.15cm} 
\pagenumbering{gobble} 

% 标题格式设置
\titleformat{\section}{\needspace{4\baselineskip}\bfseries\large}{}{0pt}{}[\vspace{1pt}\titlerule]

\titlespacing{\section}{
    -1pt
}{
    0.3 cm
}{
    0.2 cm
} 

\renewcommand\labelitemi{$\vcenter{\hbox{\small$\bullet$}}$} 

% 自定义环境
\newenvironment{highlights}{
    \begin{itemize}[
        topsep=0.10 cm,
        parsep=0.10 cm,
        partopsep=0pt,
        itemsep=0pt,
        leftmargin=0 cm + 10pt
    ]
}{
    \end{itemize}
} 

\newenvironment{highlightsforbulletentries}{
    \begin{itemize}[
        topsep=0.10 cm,
        parsep=0.10 cm,
        partopsep=0pt,
        itemsep=0pt,
        leftmargin=10pt
    ]
}{
    \end{itemize}
} 

\newenvironment{onecolentry}{
    \begin{adjustwidth}{
        0 cm + 0.00001 cm
    }{
        0 cm + 0.00001 cm
    }
}{
    \end{adjustwidth}
} 

\newenvironment{twocolentry}[2][]{
    \onecolentry
    \def\secondColumn{#2}
    \setcolumnwidth{\fill, 4.5 cm}
    \begin{paracol}{2}
}{
    \switchcolumn \raggedleft \secondColumn
    \end{paracol}
    \endonecolentry
} 

\newenvironment{header}{
    \setlength{\topsep}{0pt}\par\kern\topsep\centering\linespread{1.5}
}{
    \par\kern\topsep
} 

\let\hrefWithoutArrow\href

\begin{document}
    \newcommand{\AND}{\unskip
        \cleaders\copy\ANDbox\hskip\wd\ANDbox
        \ignorespaces
    }
    \newsavebox\ANDbox
    \sbox\ANDbox{$|$}

    \begin{header}
        \fontsize{25 pt}{25 pt}\selectfont 沈 硕

        \vspace{5 pt}

        \normalsize
        \mbox{上海}%
        \kern 5.0 pt%
        \AND%
        \kern 5.0 pt%
        \mbox{{svenshen@tencent.com}}%
        \kern 5.0 pt%
        \AND%
        \kern 5.0 pt%
        \mbox{{+86 18745029162}}%
        \kern 5.0 pt%
        \AND%
        \kern 5.0 pt%
        \mbox{\hrefWithoutArrow{https://github.com/Hyperion-shuo}{github.com/Hyperion-shuo}}%
    \end{header}

    \vspace{5 pt - 0.3 cm}

    \section{教育经历}

        \begin{twocolentry}{
            2015年9月 – 2019年5月
        }
            \textbf{哈尔滨工业大学}，本科，数字媒体技术\end{twocolentry}

        \vspace{0.10 cm}

        \begin{twocolentry}{
            2019年9月 – 2022年4月
        }
            \textbf{北京交通大学}，硕士，计算机科学与技术\end{twocolentry}

        \vspace{0.10 cm}

    
    \section{工作经历}

        \begin{twocolentry}{
            2021年6月 – 2021年9月
        }
            \textbf{强化学习算法实习生}，网易游戏 AI Lab —— 上海\end{twocolentry}

        \vspace{0.10 cm}
        
        \begin{twocolentry}{
            2022年5月 – 2023年9月
        }
            \textbf{强化学习算法工程师}，网易游戏 AI Lab —— 上海\end{twocolentry}

        \vspace{0.2 cm}

        \begin{twocolentry}{
            2023年10月 – 至今
        }
            \textbf{游戏 AI 工程师（应用研究方向）}，腾讯 IEG —— 上海\end{twocolentry}


    \section{获奖情况}
        \begin{samepage}
            \begin{twocolentry}{
                2020
            }
                \textit{KDD CUP 强化学习赛道：网约车订单派送与调度任务 (6/150)}
            \end{twocolentry}

            \begin{twocolentry}{
                2020
            }
                \textit{SMARTS DAI 自动驾驶单智能体赛道 (7/70)}
            \end{twocolentry}

            \begin{twocolentry}{
                2021
            }
                \textit{CoG FightingICE 格斗游戏 AI 竞赛 (1/15)}
            \end{twocolentry}

            \begin{twocolentry}{
                2022
            }
                \textit{CoG Google Research Football 多智能体 AI 竞赛 (1/20)}
            \end{twocolentry}

            \begin{twocolentry}{
                2023
            }
                \textit{IJCAI AI 奥林匹克竞赛 (1/40, 口头报告)}
            \end{twocolentry}

            \begin{twocolentry}{
                2023
            }
                \textit{CoG Google Research Football 多智能体 AI 竞赛 (2/20)}
            \end{twocolentry}

            \vspace{0.10 cm}
            
        \end{samepage}
    
    \section{发表论文}

        \begin{samepage}
            \begin{twocolentry}{
                2023
            }
                \textbf{Diversity is Strength: Mastering Football Full Game with Interactive Reinforcement Learning of Multiple AIs, Arxiv}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                \mbox{Chenglu Sun}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Sijia Xu} \mbox{Weidong Zhang}

                \vspace{0.10 cm}
                
        \href{https://arxiv.org/abs/2306.15903}{\underline{论文链接}}
        \end{onecolentry}
        \end{samepage}
        
        \begin{samepage}
            \begin{twocolentry}{
                2024
            }
                \textbf{Enhancing Off-Policy Constrained Reinforcement Learning through Adaptive Ensemble C Estimation, AAAI Accepted}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                \mbox{Hengrui Zhang}, \mbox{Youfang Lin}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Sheng Han}, \mbox{Kai Lv}

                \vspace{0.10 cm}
                
        \href{https://ojs.aaai.org/index.php/AAAI/article/view/30177}{\underline{论文链接}}
        \end{onecolentry}
        \end{samepage}

        \begin{samepage}
            \begin{twocolentry}{
                2024
            }
                \textbf{Enhancing AI-Bot Strength and Strategy Diversity in Adversarial Games: A Novel Deep Reinforcement Learning Framework, IEEE ToG Accepted}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                \mbox{Chenglu Sun}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Wenzhi Tao}, \mbox{Deyi Xue} and \mbox{Zixia Zhou}

                \vspace{0.10 cm}

        \href{https://ieeexplore.ieee.org/document/10812583}{\underline{论文链接}}
        \end{onecolentry}
        \end{samepage}

        \begin{samepage}
            \begin{twocolentry}{
                2025
            }
                \textbf{Noise-Resilient Symbolic Regression with Dynamic Gating Reinforcement Learning, AAAI Accepted, Oral}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                \mbox{Chenglu Sun}, \mbox{Youfang Lin}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Wenzhi Tao}, \mbox{Deyi Xue}, \mbox{Zixia Zhou}

                \vspace{0.10 cm}
                
        \href{https://arxiv.org/abs/2501.01085}{\underline{论文链接}}
        \end{onecolentry}
        \end{samepage}

        \begin{samepage}
            \begin{twocolentry}{
                2025
            }
                \textbf{Enhancing Offline Safe Reinforcement Learning with Trajectory-Constrained Diffusion Planning, AAMAS Accepted as Extended Abstracts}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                \mbox{Hengrui Zhang}, \mbox{Youfang Lin}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Hanfeng Lin}, \mbox{Peng Cheng}, \mbox{Sheng Han}, \mbox{Kai Lv}

                \vspace{0.10 cm}
                
        \end{onecolentry}
        \end{samepage}
        
        \begin{samepage}
            \begin{twocolentry}{
                2025
            }
                \textbf{Complex Instruction Following with Diverse Style Policies in Football Games, AAAI26 Accepted}
            \end{twocolentry}

            \vspace{0.10 cm}
            
            \begin{onecolentry}
                  \mbox{Chenglu Sun}, \mbox{\textbf{\textit{Shuo Shen}}}, \mbox{Haonan Hu}, \mbox{Wei Zhou} and \mbox{ Chen Chen}

                \vspace{0.10 cm}
                
        \href{https://lcdsp-webpage.github.io/LCDSP/}{\underline{项目主页}}
        \end{onecolentry}
        \end{samepage}

    
    
    \section{项目经历}
        
        \begin{twocolentry}{
        }
            \textbf{IEEE CoG2021 格斗游戏 AI 竞赛 (2021/6-2021/8)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 获得 IEEE CoG2021 格斗游戏 AI 竞赛冠军，在 PVE 速通和 PVP 三角色赛道均达到 $100\%$ 胜率。
                \item 开发了基于格斗游戏的分布式种群训练（PBT）框架，使奖励风格参数能收敛到固定值。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}

        \begin{twocolentry}{
        }
        \textbf{IEEE CoG2022 Google Research Football 多智能体 AI 竞赛 (2022/5-2022/9)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 分析 Kaggle 头部单智能体足球方案。构建特征与奖励。开发特定场景以增强开球、二过一传球等技能。通过设计不同奖励创建不同风格的模型。
                \item 创新混合对手池采样机制，集成多种算法和模型类型。实现大规模分布式 PPO 模型训练。
                \item 设计多阶段模型筛选流程：初始 Elo 筛选、特定场景技能评估、综合风格评估（进球、射门、控球、拦截）及最终专家评审，从数百个模型中选出最优候选。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}

        \begin{twocolentry}{
        }
            \textbf{大规模 SLG（在线战争策略游戏）AI 开发与部署 (2022/10-2023/9)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 主导训练环境优化、特征与奖励设计及高层动作开发。实现了 AI 战略决策的可视化评估模块。
                \item 参与 CQL 和分布式 PPO 算法开发，解决长期反馈和数据稀疏挑战。
                \item 牵头在线推理框架的开发与部署。新服 A/B 测试显示 AI 攻防能力提升。用户满意度分析表明玩家活跃度和付费率有所提高。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}

        \begin{twocolentry}{
        }
            \textbf{多风格篮球游戏 AI 机器人 (2023/10-2025/5)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 在公司自研篮球游戏中训练 1v1 和 3v3 攻防 AI。搭建训练环境、RL 分布式训练系统，设计奖励、动作和特征。使用分布式 PPO 和 Selfplay 框架进行训练和评估。
                \item 设计多种元行为及相应奖励，使 AI 能执行特定风格，如三分、上篮、中投的进攻倾向，以及篮板和盖帽的防守倾向。
                \item 集成篮球垂类微调 ASR 模型和 LLM，实现通过语音或自然语言输入控制 AI 风格和行为。
                \item 进行中的研究：遵循阵型和战术，从玩家数据中学习，以及改进多智能体协作。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}

        \begin{twocolentry}{
        }
            \textbf{NBA2KX TTS 语音合成系统开发 (2024/6-2024/9)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 处理并标注授权解说音频，进行精确标点、停顿和语音调整（如处理“儿化音”），以改善发音并减少错误。
                \item 构建合成流水线，结合提示词过滤、TTS、ASR 验证和批处理以生产高质量语音包。实施文本标准化（标点清洗、语音校正）和基于权重的长句分割策略，确保音频连贯并防止截断。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}

        \begin{twocolentry}{
        }
            \textbf{基于机器学习的 NBA2KX 画质配置推荐 (2025/3-2025/4)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 深入分析先锋测试和 S1 数据，为利益相关者可视化性能指标，主动检测帧率锁定和过热等硬件特定问题。
                \item 为超过 7000 种设备型号生成推荐画质配置，并在游戏发布期间成功部署机器学习模型预测。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}
        
        \begin{twocolentry}{
        }
            \textbf{NBA2KX 智能 QA 助手 (2025/6-2025/11)}\end{twocolentry}
        \vspace{0.10 cm}
        \begin{onecolentry}
            \begin{highlights}
                \item 设计基于 MCP 协议的多智能体系统（使用混元-turbo 模型）；实现任务规划、人设定制和安全护栏，平均响应时间达到 15秒。
                \item 构建混合检索系统（向量/ES/MySQL）配合 Reranker 模型；设计自动化流水线和零停机热更新机制，实现跨隔离环境的无缝语料库管理。
            \end{highlights}
        \end{onecolentry}
        \vspace{0.2 cm}


    \section{技术栈}
        \begin{onecolentry}
            \textbf{RL 算法：} 大规模分布式 RL 系统、Self-Play（自博弈）、Model-based RL（基于模型的 RL）、Multi-agent RL（多智能体 RL）、Offline RL（离线 RL）、RLHF、RLVR。
        \end{onecolentry}

        \vspace{0.2 cm}

        \begin{onecolentry}
            \textbf{LLMs：} Transformer 等
        \end{onecolentry}

        \vspace{0.2 cm}
        
        \begin{onecolentry}
            \textbf{编程技能：} C, Python, Torch, Tensorflow1
        \end{onecolentry}

        \vspace{0.2 cm}

        \begin{onecolentry}
            \textbf{其他技术：} Git, Linux, Vscode 
        \end{onecolentry}

\end{document}