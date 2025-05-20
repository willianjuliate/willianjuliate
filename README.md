# 👋 Hello! Welcome to my GitHub profile

## 🧑‍💻 About Me

Hey there! I'm **Willian**, but you can call me **Will**.

- 🛠️ System Analyst and passionate **Rust** programmer
- ⚙️ Tinkerer of clean code, efficient systems, and old-school simplicity
- 🧠 Always learning — currently diving into **Rust** 🦀 and **Functional Programming**
- 💬 I enjoy talking about systems architecture, performance, and timeless programming principles

## 🧰 Tech Toolbox

```rust
enum Category {
    Language,
    Runtime,
    Framework,
    OS,
    Database,
}

struct Tech {
    name: &'static str,
    icon: &'static str,
    description: &'static str,
    category: Category,
}

fn main() {
    let stack = [
        Tech {
            name: "Rust",
            icon: "🦀",
            description: "Fast and safe systems programming",
            category: Category::Language,
        },
        Tech {
            name: "C#",
            icon: "⚙️",
            description: "Robust OOP and desktop apps",
            category: Category::Language,
        },
        Tech {
            name: "JavaScript",
            icon: "🌐",
            description: "Dynamic web programming",
            category: Category::Language,
        },
        Tech {
            name: "NodeJS",
            icon: "🟩",
            description: "Backend with JavaScript",
            category: Category::Runtime,
        },
        Tech {
            name: "React",
            icon: "⚛️",
            description: "Modern web interfaces",
            category: Category::Framework,
        },
        Tech {
            name: "Linux",
            icon: "🐧",
            description: "My dev environment",
            category: Category::OS,
        },
        Tech {
            name: "PostgreSQL",
            icon: "🐘",
            description: "Reliable SQL database",
            category: Category::Database,
        },
    ];

    println!("### 🧰 My Tech Stack ###\n");

    for tech in &stack {
        let category = match tech.category {
            Category::Language => "Language",
            Category::Runtime => "Runtime",
            Category::Framework => "Framework",
            Category::OS => "Operating System",
            Category::Database => "Database",
        };

        println!(
            "{} {:<12} ({}) - {}",
            tech.icon, tech.name, category, tech.description
        );
    }
}
