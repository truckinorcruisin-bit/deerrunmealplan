<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heart-Healthy Meal Plans for Dad</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
            background: #f5f5f0;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
        }

        header {
            background: linear-gradient(135deg, #2c5f7c 0%, #3a7ca5 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: normal;
        }

        header p {
            font-size: 1.2em;
            opacity: 0.95;
        }

        nav {
            background: #2c5f7c;
            padding: 15px;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav select {
            width: 100%;
            padding: 12px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            background: white;
            cursor: pointer;
        }

        .content {
            padding: 40px 30px;
        }

        .page {
            display: none;
            animation: fadeIn 0.3s;
        }

        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h2 {
            color: #2c5f7c;
            font-size: 2em;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #3a7ca5;
        }

        h3 {
            color: #3a7ca5;
            font-size: 1.5em;
            margin-top: 30px;
            margin-bottom: 15px;
        }

        h4 {
            color: #2c5f7c;
            font-size: 1.2em;
            margin-top: 25px;
            margin-bottom: 10px;
        }

        .intro-section {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 8px;
            margin-bottom: 30px;
            border-left: 4px solid #3a7ca5;
        }

        ul {
            margin-left: 25px;
            margin-bottom: 20px;
        }

        li {
            margin-bottom: 10px;
        }

        .grocery-list {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        .grocery-category {
            margin-bottom: 20px;
        }

        .grocery-category h4 {
            color: #2c5f7c;
            margin-top: 0;
            margin-bottom: 10px;
            font-size: 1.1em;
        }

        .grocery-category ul {
            margin-left: 0;
            list-style: none;
        }

        .grocery-item {
            display: flex;
            align-items: center;
            padding: 12px;
            margin-bottom: 8px;
            background: white;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.2s;
            border: 2px solid transparent;
        }

        .grocery-item:hover {
            border-color: #3a7ca5;
            transform: translateX(2px);
        }

        .grocery-item.checked {
            background: #e8f5e9;
            border-color: #4caf50;
            opacity: 0.7;
        }

        .grocery-item.checked label {
            text-decoration: line-through;
            color: #666;
        }

        .grocery-item input[type="checkbox"] {
            width: 24px;
            height: 24px;
            margin-right: 12px;
            cursor: pointer;
            flex-shrink: 0;
        }

        .grocery-item label {
            cursor: pointer;
            flex-grow: 1;
            font-size: 16px;
            user-select: none;
        }

        .clear-checks-btn {
            background: #ff5722;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 14px;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 15px;
        }

        .clear-checks-btn:hover {
            background: #e64a19;
        }

        .meal-card {
            background: white;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .meal-card h4 {
            margin-top: 0;
            color: #2c5f7c;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .meal-label {
            background: #3a7ca5;
            color: white;
            padding: 3px 10px;
            border-radius: 4px;
            font-size: 0.85em;
            font-weight: normal;
        }

        .meal-instructions {
            margin-top: 10px;
            color: #555;
        }

        .tip-box {
            background: #fff9e6;
            border-left: 4px solid #ffc107;
            padding: 15px;
            margin: 15px 0;
            border-radius: 4px;
        }

        .tip-box strong {
            color: #f57c00;
        }

        .cook-extra {
            background: #e8f5e9;
            border-left: 4px solid #4caf50;
            padding: 15px;
            margin: 10px 0;
            border-radius: 4px;
            font-weight: bold;
        }

        .flavor-tip {
            background: #f3e5f5;
            border-left: 4px solid #9c27b0;
            padding: 12px;
            margin: 10px 0;
            border-radius: 4px;
            font-style: italic;
        }

        strong {
            color: #2c5f7c;
        }

        .print-button {
            background: #4caf50;
            color: white;
            border: none;
            padding: 12px 24px;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 20px;
            display: inline-block;
        }

        .print-button:hover {
            background: #45a049;
        }

        @media print {
            nav, .print-button {
                display: none;
            }
            .page {
                display: block !important;
                page-break-after: always;
            }
            body {
                background: white;
            }
            .container {
                box-shadow: none;
            }
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 1.8em;
            }
            .content {
                padding: 20px 15px;
            }
        }

        footer {
            background: #2c5f7c;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>♥ Heart-Healthy Meal Plans</h1>
            <p>A Simple Guide to Easy Shopping & Delicious Eating</p>
        </header>

        <nav>
            <select id="pageSelector" onchange="changePage()">
                <option value="intro">How to Use This Guide</option>
                <option value="week1-grocery">Week 1: Mediterranean - Grocery List</option>
                <option value="week1-meals">Week 1: Mediterranean - Meals</option>
                <option value="week2-grocery">Week 2: Tex-Mex - Grocery List</option>
                <option value="week2-meals">Week 2: Tex-Mex - Meals</option>
                <option value="week3-grocery">Week 3: Comfort Classics - Grocery List</option>
                <option value="week3-meals">Week 3: Comfort Classics - Meals</option>
                <option value="week4-grocery">Week 4: Asian-Inspired - Grocery List</option>
                <option value="week4-meals">Week 4: Asian-Inspired - Meals</option>
                <option value="week5-grocery">Week 5: Italian Inspired - Grocery List</option>
                <option value="week5-meals">Week 5: Italian Inspired - Meals</option>
                <option value="tips">Quick Tips & Cooking Guide</option>
            </select>
        </nav>

        <div class="content">
            <!-- INTRO PAGE -->
            <div id="intro" class="page active">
                <h2>How to Use This Guide</h2>
                
                <div class="intro-section">
                    <p><strong>Welcome!</strong> This guide contains <strong>5 weekly meal plans</strong> that rotate to keep things interesting while staying simple.</p>
                </div>

                <h3>Each Plan Includes:</h3>
                <ul>
                    <li>A <strong>one-page grocery list</strong> with everything you need</li>
                    <li>A <strong>one-page meal plan</strong> showing what to eat for lunch and dinner each day</li>
                    <li><strong>Detailed cooking instructions</strong> with temperatures, times, and quantities</li>
                    <li><strong>Leftovers built in</strong> - cook once, eat multiple times!</li>
                </ul>

                <div class="intro-section">
                    <h3>The Pattern:</h3>
                    <p><strong>Shop once, eat well all week.</strong> Each plan uses overlapping ingredients so nothing goes to waste, and meals are designed to be quick and satisfying.</p>
                </div>

                <h3>Pro Tips:</h3>
                <ul>
                    <li>Start with Week 1, then rotate through the plans</li>
                    <li>By Week 6, you're back to Week 1 and it feels fresh again!</li>
                    <li>Shop on the same day each week - make it a routine</li>
                    <li>When you see <strong>"COOK EXTRA"</strong> notes, follow them - you're setting yourself up for easy meals later</li>
                </ul>

                <button class="print-button" onclick="window.print()">Print Entire Guide</button>
            </div>

            <!-- WEEK 1 GROCERY -->
            <div id="week1-grocery" class="page">
                <h2>Week 1: Mediterranean Basics</h2>
                <h3>Grocery List</h3>

                <div class="grocery-list">
                    <div class="grocery-category">
                        <h4>Proteins:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lb chicken breast (skinless)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lb ground turkey (93% lean or leaner)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 can chickpeas (no salt added or low sodium)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 dozen eggs</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>8 oz feta cheese (reduced-fat)</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Vegetables:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>2 bags mixed salad greens</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>3 large tomatoes</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>2 cucumbers</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 red onion</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 bell pepper (any color)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>3 zucchini</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 bag baby carrots</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lemon</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Pantry & Staples:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Whole wheat pita bread</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Brown rice</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Extra virgin olive oil</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Hummus (1 container)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Kalamata olives (1 jar)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Balsamic vinegar</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Garlic (fresh or minced jar)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Dried oregano</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Extras:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Plain non-fat Greek yogurt</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Fresh or dried parsley</label>
                            </li>
                        </ul>
                    </div>
                    
                    <button class="clear-checks-btn" onclick="clearAllChecks('week1-grocery')">Clear All Checks</button>
                </div>
            </div>

            <!-- WEEK 1 MEALS -->
            <div id="week1-meals" class="page">
                <h2>Week 1: Mediterranean Basics</h2>
                <h3>Daily Meals</h3>

                <div class="meal-card">
                    <h4>Monday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Greek salad with chickpeas, tomatoes, cucumber, feta</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Mix 2 cups salad greens, ½ can drained chickpeas, 1 chopped tomato, ½ sliced cucumber, 2 tablespoons crumbled feta. Dress with 1 tablespoon extra virgin olive oil, squeeze of lemon, pinch of oregano, salt and pepper. Serve with 1 whole wheat pita on the side.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Grilled chicken with roasted zucchini and brown rice</strong></p>
                    <div class="cook-extra">
                        🍗 COOK EXTRA CHICKEN - Grill or bake 3 chicken breasts (you'll use the extras this week!)
                    </div>
                    <div class="meal-instructions">
                        <em>How to make:</em> Season chicken breasts with extra virgin olive oil, garlic, oregano, salt and pepper. Bake at 400°F for 20-25 minutes.<br><br>
                        Slice 2 zucchini lengthwise, toss with 1 tablespoon extra virgin olive oil, salt, pepper. Roast at 400°F for 20 minutes alongside chicken.
                    </div>
                    <div class="cook-extra">
                        🍚 MAKE EXTRA RICE - Cook 2 cups brown rice to use throughout the week (2:1 water to rice ratio, simmer 40-45 minutes)
                    </div>
                    <div class="meal-instructions">
                        <em>Eat tonight:</em> 1 chicken breast, half the zucchini, 1 cup cooked rice
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Tuesday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Chicken pita wrap with hummus and veggies</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Slice 1 leftover chicken breast. Warm 1 pita, spread with 2 tablespoons hummus, add chicken, 1 cup greens, chopped cucumber and tomato. Wrap it up!
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Turkey and vegetable stir-fry over brown rice</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Heat 1 tablespoon extra virgin olive oil in a large skillet over medium-high heat. Add ½ lb ground turkey, break apart and cook 5-7 minutes until browned. Add 1 sliced bell pepper, 1 sliced zucchini, ½ sliced onion. Cook 5 minutes until tender. Season with garlic, salt, pepper, and a splash of balsamic vinegar.<br><br>
                        Serve over 1 cup reheated brown rice (from Monday).
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Wednesday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Greek yogurt bowl with olives, carrots, and hummus</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Scoop 1 cup non-fat Greek yogurt into a bowl. Drizzle with extra virgin olive oil and sprinkle with oregano. Serve with 8-10 baby carrots, handful of olives, 2 tablespoons hummus, and 1 pita cut into triangles for dipping.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Baked chicken with tomato, garlic, and oregano</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Use your last leftover chicken breast. Place in a baking dish, top with 1 chopped tomato, 2 minced garlic cloves, 1 teaspoon oregano, drizzle of extra virgin olive oil. Bake at 375°F for 15 minutes to reheat and let flavors meld.<br><br>
                        Sauté remaining zucchini slices in 1 teaspoon extra virgin olive oil over medium heat, 5-7 minutes. Season with salt and pepper.
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Thursday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Turkey and veggie pita pocket</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Heat 1 pita. Fill with ¼ lb cooked ground turkey (leftover from Tuesday), 1 cup mixed greens, chopped cucumber, chopped tomato, 2 tablespoons non-fat Greek yogurt as a creamy sauce.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Mediterranean scrambled eggs with tomatoes and feta</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Scramble 3 eggs in a pan with 1 teaspoon olive oil over medium heat. When almost done, add 1 chopped tomato, handful of spinach (wilts quickly), and 2 tablespoons crumbled feta. Season with pepper.<br><br>
                        Serve with remaining brown rice or a pita on the side.
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Friday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Chickpea and vegetable salad</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Combine remaining chickpeas (about ½ can), 1 cup mixed greens, remaining cucumber and tomatoes (diced), ¼ sliced red onion. Dress with juice of ½ lemon, 1 tablespoon olive oil, chopped parsley, salt and pepper.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Turkey burger patties with roasted vegetables</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Form remaining ground turkey (about ¼ lb) into 2 small patties. Season with garlic, oregano, salt and pepper. Pan-fry in 1 teaspoon olive oil over medium heat, 4-5 minutes per side.<br><br>
                        Roast any remaining vegetables (bell pepper, zucchini, onion) tossed in olive oil at 400°F for 20 minutes.
                    </div>
                </div>

                <div class="tip-box">
                    <strong>Weekend Flexibility:</strong> Mix remaining proteins with rice, beans, and vegetables for easy bowls or wraps. These ingredients freeze well in small portions!
                </div>
            </div>

<!-- WEEK 2 GROCERY -->
        <div id="week2-grocery" class="page">
            <h2>Week 2: Tex-Mex Favorites</h2>
            <h3>Grocery List</h3>

            <div class="grocery-list">
                <div class="grocery-category">
                    <h4>Proteins:</h4>
                    <ul>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 lb ground beef (90% lean or leaner) or ground turkey</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 lb boneless skinless chicken thighs</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 can black beans (no salt added or low sodium)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 can pinto beans (no salt added or low sodium)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Shredded cheese (reduced-fat cheddar)</label>
                        </li>
                    </ul>
                </div>

                <div class="grocery-category">
                    <h4>Vegetables:</h4>
                    <ul>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>2 bell peppers (red and green)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>3 tomatoes</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 large onion</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 bag baby spinach</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 avocado</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>1 lime</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Jalapeño (optional)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Cilantro (fresh)</label>
                        </li>
                    </ul>
                </div>

                <div class="grocery-category">
                    <h4>Pantry & Staples:</h4>
                    <ul>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Corn tortillas (small, whole grain)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Brown rice</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Salsa (jar, low sodium)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Low-sodium taco seasoning</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Extra virgin olive oil or cooking spray</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Garlic powder</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Cumin</label>
                        </li>
                    </ul>
                </div>

                <div class="grocery-category">
                    <h4>Extras:</h4>
                    <ul>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Plain non-fat Greek yogurt (for sour cream substitute)</label>
                        </li>
                        <li class="grocery-item" onclick="toggleCheck(this)">
                            <input type="checkbox" onclick="event.stopPropagation()">
                            <label>Hot sauce (optional)</label>
                        </li>
                    </ul>
                </div>
                
                <button class="clear-checks-btn" onclick="clearAllChecks('week2-grocery')">Clear All Checks</button>
            </div>
        </div>

        <!-- WEEK 2 MEALS -->
        <div id="week2-meals" class="page">
            <h2>Week 2: Tex-Mex Favorites</h2>
            <h3>Daily Meals</h3>

            <div class="meal-card">
                <h4>Monday</h4>
                
                <p><span class="meal-label">LUNCH</span> <strong>Black bean and rice bowl</strong></p>
                <div class="cook-extra">
                    🍚 COOK EXTRA RICE TODAY - Make 2 cups dry rice for the week
                </div>
                <div class="meal-instructions">
                    <em>How to make:</em> Reheat 1 cup cooked brown rice. Top with ½ can drained black beans (warmed), 1 diced tomato, 2 tablespoons salsa, 2 tablespoons shredded cheese. Add hot sauce if you like heat!
                </div>

                <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Ground beef tacos with peppers and onions</strong></p>
                <div class="cook-extra">
                    🥩 COOK THE FULL POUND - You'll use half tonight and save the rest
                </div>
                <div class="meal-instructions">
                    <em>How to make:</em> Brown 1 lb ground beef in a large skillet over medium-high heat, 7-8 minutes. Drain any excess fat. Add 1 packet taco seasoning (or DIY: 1 tablespoon chili powder, 1 teaspoon cumin, ½ teaspoon garlic powder, salt). Add ½ cup water, simmer 5 minutes.<br><br>
                    Meanwhile, sauté 1 sliced bell pepper and ½ sliced onion in 1 teaspoon olive oil until tender, about 8 minutes.<br><br>
                    <em>Eat tonight:</em> Use half the taco meat. Warm 3-4 corn tortillas. Fill with meat, peppers, onions, salad greens, and a dollop of Greek yogurt.
                </div>
            </div>

            <div class="meal-card">
                <h4>Tuesday</h4>
                
                <p><span class="meal-label">LUNCH</span> <strong>Taco salad with beans and salsa dressing</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Arrange 2 cups spinach on a plate. Top with ⅓ cup reheated taco meat, remaining black beans, 1 diced tomato, and 2 tablespoons salsa as dressing. Add a squeeze of lime if you have it.
                </div>

                <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Grilled chicken thighs with peppers and pinto beans</strong></p>
                <div class="cook-extra">
                    🍗 COOK ALL 4 THIGHS - Save extras for later this week
                </div>
                <div class="meal-instructions">
                    <em>How to make:</em> Season 1 lb chicken thighs with olive oil, cumin, garlic powder, salt and pepper. Grill or bake at 400°F for 25-30 minutes until internal temp reaches 165°F.<br><br>
                    Sauté remaining bell pepper and onion half in 1 tablespoon olive oil, 8-10 minutes.<br><br>
                    Warm ½ can pinto beans on the stove with a pinch of cumin.<br><br>
                    <em>Eat tonight:</em> 2 chicken thighs with half the vegetables and beans.
                </div>
            </div>

            <div class="meal-card">
                <h4>Wednesday</h4>
                
                <p><span class="meal-label">LUNCH</span> <strong>Bean and veggie burrito bowl</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Build your bowl with 1 cup reheated rice, remaining pinto beans (warmed), leftover sautéed peppers and onions, 3 tablespoons salsa, 2 tablespoons cheese. Top with cilantro if you have it.
                </div>

                <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Chicken fajitas with corn tortillas</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Slice 1 leftover chicken thigh into strips. Sauté in a pan with any remaining peppers/onions (or slice a fresh one), 1 teaspoon extra virgin olive oil, cumin, and chili powder, 5-7 minutes.<br><br>
                    Warm 3-4 corn tortillas. Serve chicken and veggies with tortillas, salsa, and non-fat Greek yogurt.
                </div>
                <div class="flavor-tip">
                    <strong>Flavor twist:</strong> Add a squeeze of lime and fresh cilantro for brighter flavor!
                </div>
            </div>

            <div class="meal-card">
                <h4>Thursday</h4>
                
                <p><span class="meal-label">LUNCH</span> <strong>Chicken and spinach salad with avocado</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Slice remaining chicken thigh. Arrange 2 cups spinach, add chicken, any leftover beans, 1 diced tomato, ½ sliced avocado. Squeeze lime over everything, drizzle with 1 tablespoon extra virgin olive oil, sprinkle with salt and pepper.
                </div>

                <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Beef and bean skillet over rice</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Reheat remaining taco meat in a skillet. Add 1 diced tomato, any leftover beans, ½ teaspoon cumin, pinch of chili powder. Stir and cook 5 minutes until heated through.<br><br>
                    Serve over 1 cup reheated rice. Top with cheese and salsa if desired.
                </div>
            </div>

            <div class="meal-card">
                <h4>Friday</h4>
                
                <p><span class="meal-label">LUNCH</span> <strong>Quesadilla with chicken or beans</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Heat a skillet over medium heat. Place 1 corn tortilla in pan, sprinkle with 3 tablespoons cheese, add any leftover chicken (shredded) or beans, top with another tortilla. Cook 2-3 minutes per side until golden and cheese melts. Cut into wedges. Serve with salsa.
                </div>

                <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Mexican-style scrambled eggs</strong></p>
                <div class="meal-instructions">
                    <em>How to make:</em> Scramble 3 eggs in 1 teaspoon olive oil. Add any remaining peppers/onions, a few tablespoons of beans, cook until eggs are set. Top with salsa and cheese.<br><br>
                    Serve with warm corn tortillas on the side.
                </div>
            </div>

            <!-- ============================================================ -->
<!-- WEEK 3 GROCERY LIST -->
<!-- ============================================================ -->

<div id="week3-grocery" class="page">
    <h2>Week 3: Comfort Classics</h2>
    <h3>Grocery List</h3>

    <div class="grocery-list">
        <div class="grocery-category">
            <h4>Proteins:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb lean ground beef or turkey (90% lean or leaner)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb boneless pork chops (trimmed of visible fat)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 can white beans (no salt added or low sodium)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>4 salmon fillets (fresh or frozen, wild-caught preferred)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Eggs (½ dozen)</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Vegetables:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 bag mixed salad greens</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>3 sweet potatoes</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb green beans</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>2 heads broccoli</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>3 carrots</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>2 onions</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Garlic (fresh or jar)</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Pantry & Staples:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Whole wheat pasta</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Brown rice</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Low-sodium marinara sauce (jar)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Extra virgin olive oil</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Low-sodium chicken or vegetable broth</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Low-sodium soy sauce</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Dijon mustard</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Dried thyme and rosemary</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Extras:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Parmesan cheese (small amount)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Lemon</label>
                </li>
            </ul>
        </div>
        
        <button class="clear-checks-btn" onclick="clearAllChecks('week3-grocery')">Clear All Checks</button>
    </div>
</div>

<!-- ============================================================ -->
<!-- WEEK 3 MEALS -->
<!-- ============================================================ -->

<div id="week3-meals" class="page">
    <h2>Week 3: Comfort Classics</h2>
    <h3>Daily Meals</h3>

    <div class="meal-card">
        <h4>Monday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>White bean and vegetable soup</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> In a pot, sauté 1 diced onion and 2 sliced carrots in 1 tablespoon extra virgin olive oil over medium heat, 5 minutes. Add 2 minced garlic cloves, cook 1 minute. Add 1 can drained white beans, 3 cups low-sodium chicken or vegetable broth, 1 teaspoon dried thyme. Simmer 15 minutes. Season with salt and pepper.<br><br>
            <em>Makes:</em> About 3 servings. Save extras in fridge for quick lunches!
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Baked salmon with roasted sweet potato and steamed broccoli</strong></p>
        <div class="cook-extra">
            🐟 BAKE ALL 4 SALMON FILLETS - You'll use extras this week
        </div>
        <div class="meal-instructions">
            <em>How to make:</em> Place salmon on a baking sheet, drizzle with extra virgin olive oil, season with salt, pepper, and lemon juice. Bake at 400°F for 12-15 minutes until flaky.<br><br>
            Cut 2 sweet potatoes into 1-inch cubes, toss with 1 tablespoon extra virgin olive oil, salt, pepper. Roast at 400°F for 25-30 minutes, flipping halfway.<br><br>
            Steam 1 head of broccoli (cut into florets) for 5-7 minutes until tender. Season with lemon and olive oil.<br><br>
            <em>Eat tonight:</em> 1 salmon fillet, half the sweet potato, half the broccoli.
        </div>
    </div>

    <div class="meal-card">
        <h4>Tuesday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Leftover salmon over mixed greens with lemon</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Flake 1 cold salmon fillet over 2 cups mixed greens. Add leftover roasted sweet potato cubes, drizzle with 1 tablespoon extra virgin olive oil and juice of ½ lemon. Season with salt and pepper.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Lean beef pasta with marinara and green beans</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Cook ½ lb whole wheat pasta according to package directions. Meanwhile, brown ½ lb ground beef in a skillet over medium-high heat, 7-8 minutes. Drain excess fat. Add 1½ cups marinara sauce, simmer 5 minutes.<br><br>
            Steam or boil ½ lb green beans for 5-7 minutes until tender. Season with garlic powder and a drizzle of extra virgin olive oil.<br><br>
            <em>Eat tonight:</em> Half the pasta with meat sauce, and half the green beans.<br><br>
            <em>Save:</em> Remaining pasta and meat sauce for Thursday, remaining beef for tomorrow.
        </div>
    </div>

    <div class="meal-card">
        <h4>Wednesday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Sweet potato and white bean mash with salad</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Mash remaining roasted sweet potato with ½ cup white beans (warmed). Season with salt, pepper, and a pinch of rosemary. Serve with 2 cups mixed greens tossed in extra virgin olive oil and vinegar.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Pork chops with roasted carrots and broccoli</strong></p>
        <div class="cook-extra">
            🥩 COOK ALL 4 PORK CHOPS - Save for Friday
        </div>
        <div class="meal-instructions">
            <em>How to make:</em> Season pork chops with salt, pepper, garlic powder, and thyme. Heat 1 tablespoon extra virgin olive oil in an oven-safe skillet over medium-high heat. Sear chops 3 minutes per side, then transfer skillet to 375°F oven for 8-10 minutes until internal temp reaches 145°F.<br><br>
            Slice remaining carrots, toss with olive oil, salt, pepper. Roast at 375°F for 20-25 minutes.<br><br>
            Steam remaining broccoli florets for 5-7 minutes.<br><br>
            <em>Eat tonight:</em> 1 pork chop with half the vegetables.
        </div>
    </div>

    <div class="meal-card">
        <h4>Thursday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Pasta salad with veggies and white beans</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Use leftover pasta (cold is fine), add remaining white beans, any leftover roasted carrots or green beans, 2 tablespoons extra virgin olive oil, 1 tablespoon vinegar, salt, pepper. Toss together.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Ground beef and vegetable stir-fry over rice</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Heat 1 tablespoon extra virgin olive oil in a skillet. Add remaining ground beef (broken up), remaining green beans (cut in half), ½ sliced onion. Stir-fry 5-7 minutes. Season with garlic, low-sodium soy sauce, and pepper.<br><br>
            Cook 1 cup brown rice according to package, or use pre-cooked if you have it.
        </div>
        <div class="flavor-tip">
            <strong>Flavor variation:</strong> Add a splash of Dijon mustard or balsamic vinegar for a tangy twist!
        </div>
    </div>

    <div class="meal-card">
        <h4>Friday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Leftover pork sliced over greens with roasted vegetables</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Slice 1 cold pork chop over 2 cups mixed greens. Add any remaining roasted carrots or broccoli. Dress with 1 tablespoon extra virgin olive oil, juice of ½ lemon, and Dijon mustard.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Simple salmon cakes with steamed vegetables</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Flake remaining salmon (about 1 fillet's worth), mix with 1 beaten egg, 2 tablespoons breadcrumbs (or crushed crackers), minced garlic, salt, pepper. Form into 3 small patties. Pan-fry in 1 tablespoon extra virgin olive oil over medium heat, 3-4 minutes per side until golden.<br><br>
            Steam any remaining vegetables or open a can of green beans.
        </div>
    </div>

    <div class="tip-box">
        <strong>Weekend Flexibility:</strong> Use remaining pork chop for a simple salad or reheat with vegetables. Leftover soup makes an easy lunch!
    </div>
</div>

<!-- ============================================================ -->
<!-- WEEK 4 GROCERY LIST -->
<!-- ============================================================ -->

<div id="week4-grocery" class="page">
    <h2>Week 4: Asian-Inspired</h2>
    <h3>Grocery List</h3>

    <div class="grocery-list">
        <div class="grocery-category">
            <h4>Proteins:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb chicken breast (skinless)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb shrimp (frozen, peeled and deveined)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 lb extra-firm tofu</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 dozen eggs</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Vegetables:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 bag shredded cabbage or coleslaw mix</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>2 bell peppers</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 head broccoli</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 package snap peas or green beans</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>3 carrots</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>1 bunch green onions</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Fresh ginger (small knob)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Garlic</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Pantry & Staples:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Brown rice</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Rice vinegar</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Low-sodium soy sauce</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Sesame oil (small bottle)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Honey</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Extra virgin olive oil</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Cornstarch</label>
                </li>
            </ul>
        </div>

        <div class="grocery-category">
            <h4>Extras:</h4>
            <ul>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Sesame seeds (optional)</label>
                </li>
                <li class="grocery-item" onclick="toggleCheck(this)">
                    <input type="checkbox" onclick="event.stopPropagation()">
                    <label>Sriracha or chili flakes (optional)</label>
                </li>
            </ul>
        </div>
        
        <button class="clear-checks-btn" onclick="clearAllChecks('week4-grocery')">Clear All Checks</button>
    </div>
</div>

<!-- ============================================================ -->
<!-- WEEK 4 MEALS -->
<!-- ============================================================ -->

<div id="week4-meals" class="page">
    <h2>Week 4: Asian-Inspired</h2>
    <h3>Daily Meals</h3>

    <div class="meal-card">
        <h4>Monday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Asian-style cabbage salad with sesame-ginger dressing</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Combine 2 cups shredded cabbage, 1 shredded carrot, 2 sliced green onions. For dressing: whisk 1 tablespoon sesame oil, 1 tablespoon rice vinegar, 1 teaspoon honey, ½ teaspoon grated ginger, pinch of salt. Toss salad with dressing. Top with sesame seeds if you have them.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Chicken stir-fry with broccoli, bell peppers, and snap peas</strong></p>
        <div class="cook-extra">
            🍗 COOK ALL THE CHICKEN - You'll use extras this week
        </div>
        <div class="meal-instructions">
            <em>How to make:</em> Cut 1 lb chicken breast into bite-sized pieces. Heat 1 tablespoon olive oil in a large skillet or wok over high heat. Add chicken, cook 5-6 minutes until cooked through. Remove chicken, set aside.<br><br>
            In same pan, add 1 tablespoon oil, 2 cups broccoli florets, 1 sliced bell pepper, 1 cup snap peas. Stir-fry 5-7 minutes until tender-crisp.<br><br>
            Make sauce: mix 2 tablespoons low-sodium soy sauce, 1 tablespoon honey, 1 teaspoon grated ginger, 1 minced garlic clove. Pour over vegetables, add chicken back in, toss everything together.
        </div>
        <div class="cook-extra">
            🍚 COOK 2 CUPS BROWN RICE - Make extras for the week
        </div>
        <div class="meal-instructions">
            <em>Eat tonight:</em> Half the stir-fry over 1 cup rice.<br>
            <em>Save:</em> Remaining stir-fry for Wednesday, remaining chicken for tomorrow.
        </div>
    </div>

    <div class="meal-card">
        <h4>Tuesday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Leftover chicken and vegetables over cabbage</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Arrange 2 cups shredded cabbage on a plate. Top with ⅓ of leftover stir-fry (cold or reheated). Drizzle with extra soy sauce mixed with a little rice vinegar and sesame oil.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Garlic-ginger shrimp with stir-fried vegetables</strong></p>
        <div class="cook-extra">
            🍤 COOK ALL THE SHRIMP - Save some for Thursday
        </div>
        <div class="meal-instructions">
            <em>How to make:</em> Thaw if frozen, pat dry. Heat 1 tablespoon olive oil in a skillet over medium-high heat. Add ½ lb shrimp, 2 minced garlic cloves, 1 teaspoon grated ginger, cook 2-3 minutes per side until pink.<br><br>
            Stir-fry remaining bell pepper, broccoli, and snap peas in 1 tablespoon oil with garlic, 5-7 minutes.<br><br>
            Season with low-sodium soy sauce and sesame oil.<br><br>
            <em>Eat tonight:</em> ⅔ of the shrimp with half the vegetables over 1 cup reheated rice.<br>
            <em>Save:</em> Remaining shrimp for Thursday.
        </div>
    </div>

    <div class="meal-card">
        <h4>Wednesday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Egg fried rice with mixed vegetables</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Heat 1 tablespoon olive or sesame oil in a skillet. Add 1 diced carrot, cook 3 minutes. Add 2 cups leftover rice (cold rice works best for fried rice), break up any clumps. Stir-fry 3-4 minutes. Push rice to the side, crack 2 eggs into the pan, scramble them, then mix into rice. Add 2 sliced green onions, splash of low-sodium soy sauce.<br><br>
            <em>Makes:</em> A generous portion - eat what you want, save the rest.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Baked tofu with sesame-soy glaze and steamed vegetables</strong></p>
        <div class="cook-extra">
            🥡 PREPARE ALL THE TOFU - Save half for Friday
        </div>
        <div class="meal-instructions">
            <em>How to make:</em> Drain tofu, press between paper towels to remove excess water. Cut into ½-inch thick slabs. Arrange on a baking sheet, brush with mixture of 2 tablespoons low-sodium soy sauce, 1 tablespoon sesame oil, 1 teaspoon honey, minced garlic. Bake at 400°F for 25-30 minutes, flipping halfway, until golden and slightly crispy.<br><br>
            Steam remaining broccoli and slice and steam remaining carrots, 5-7 minutes.<br><br>
            <em>Eat tonight:</em> Half the tofu with half the vegetables over rice.<br>
            <em>Save:</em> Remaining tofu for Friday.
        </div>
    </div>

    <div class="meal-card">
        <h4>Thursday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Shrimp and cabbage salad with rice vinegar dressing</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Toss 2 cups cabbage with remaining shrimp, 1 shredded carrot, 2 sliced green onions. Dress with 1 tablespoon rice vinegar, 1 teaspoon sesame oil, pinch of salt. Sprinkle with sesame seeds.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Chicken and vegetable stir-fry over rice</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Reheat remaining stir-fry from Monday. Serve over 1 cup reheated rice.
        </div>
        <div class="flavor-tip">
            <strong>Flavor boost:</strong> Add a splash more soy sauce, fresh ginger, or a drizzle of sriracha if you like spice!
        </div>
    </div>

    <div class="meal-card">
        <h4>Friday</h4>
        
        <p><span class="meal-label">LUNCH</span> <strong>Tofu scramble with vegetables and soy sauce</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> Crumble remaining tofu with a fork. Sauté in 1 tablespoon oil with any remaining vegetables (cabbage, carrots, green onions) for 5-7 minutes. Season with low-sodium soy sauce, garlic powder, and a pinch of turmeric for color.
        </div>
        
        <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Simple rice bowl with remaining proteins and vegetables</strong></p>
        <div class="meal-instructions">
            <em>How to make:</em> If you have any shrimp or chicken left, make a quick stir-fry. If not, use remaining tofu or make egg fried rice with whatever vegetables remain.<br><br>
            The beauty of this week: everything mixes and matches! Use what you have.
        </div>
    </div>

    <div class="tip-box">
        <strong>Weekend Flexibility:</strong> Create simple rice bowls with any remaining proteins and vegetables. Cabbage keeps well - make another fresh salad with sesame dressing!
    </div>
</div>


            <div class="tip-box">
                <strong>

            <!-- Continue with remaining weeks... -->
            <div id="week3-grocery" class="page">
                <h2>Week 3: Comfort Classics</h2>
                <h3>Grocery List</h3>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>For the complete Week 3-5 grocery lists and meals, refer to the original booklet content. This HTML template shows the structure for easy web hosting!</em>
                </p>
            </div>

            <div id="week3-meals" class="page">
                <h2>Week 3: Comfort Classics - Meals</h2>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>Detailed meal instructions for Week 3 would go here following the same format as Weeks 1-2.</em>
                </p>
            </div>

            <div id="week4-grocery" class="page">
                <h2>Week 4: Asian-Inspired</h2>
                <h3>Grocery List</h3>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>Week 4 grocery list content goes here.</em>
                </p>
            </div>

            <div id="week4-meals" class="page">
                <h2>Week 4: Asian-Inspired - Meals</h2>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>Week 4 detailed meal instructions go here.</em>
                </p>
            </div>

            <div id="week5-grocery" class="page">
                <h2>Week 5: Italian Inspired</h2>
                <h3>Grocery List</h3>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>Week 5 grocery list content goes here.</em>
                </p>
            </div>

            <div id="week5-meals" class="page">
                <h2>Week 5: Italian Inspired - Meals</h2>
                <p style="padding: 20px; background: #f8f9fa; border-radius: 8px;">
                    <em>Week 5 detailed meal instructions go here.</em>
                </p>
            </div>

            <!-- TIPS PAGE -->
            <div id="tips" class="page">
                <h2>Quick Tips for Success</h2>

                <div class="tip-box">
                    <strong>1. Shop on the same day each week</strong> - Make it a routine (Sunday works great for many people).
                </div>

                <div class="tip-box">
                    <strong>2. Prep a little on shopping day</strong> - Wash and chop some vegetables, cook a batch of brown rice to refrigerate.
                </div>

                <div class="tip-box">
                    <strong>3. Keep it simple</strong> - These meals are forgiving. Swap vegetables based on what looks good or what's on sale.
                </div>

                <div class="tip-box">
                    <strong>4. Batch cooking helps</strong> - Cook extra chicken or rice at dinner to use for next day's lunch.
                </div>

                <div class="tip-box">
                    <strong>5. Hydrate</strong> - Keep water handy throughout the day. Your heart will thank you!
                </div>

                <div class="tip-box">
                    <strong>6. The staples stay the same</strong> - Olive oil, garlic, onions, and basic seasonings appear in every plan. Stock these once.
                </div>

                <h3 style="margin-top: 40px;">Heart-Healthy Cooking Tips</h3>

                <ul style="margin-top: 20px;">
                    <li><strong>Grill, bake, or sauté instead of frying</strong> - Use cooking spray or a small amount of olive oil.</li>
                    <li><strong>Season boldly</strong> - Herbs, spices, garlic, lemon, and vinegar add tons of flavor without salt.</li>
                    <li><strong>Choose whole grains</strong> - Brown rice and whole wheat products are better for your heart.</li>
                    <li><strong>Load up on vegetables</strong> - They should fill half your plate.</li>
                    <li><strong>Watch portions with cheese</strong> - A little goes a long way for flavor.</li>
                    <li><strong>Read labels</strong> - Look for low-sodium options when buying canned goods and seasonings.</li>
                </ul>

                <div class="intro-section" style="margin-top: 40px; text-align: center;">
                    <h2 style="border: none; color: #2c5f7c;">You've Got This! ♥</h2>
                    <p style="font-size: 1.1em; margin-top: 15px;">These plans are designed to make your life easier, keep your heart healthy, and make grocery shopping feel like a breeze. Stick with the pattern, rotate through the weeks, and enjoy the variety.</p>
                    <p style="font-size: 1.1em; margin-top: 10px;"><strong>Remember, you're taking great care of yourself one meal at a time.</strong></p>
                </div>
            </div>
        </div>

        <footer>
            <p>Made with ♥ for Dad</p>
            <p style="margin-top: 10px; font-size: 0.9em;">Shop once. Eat well. Take care of your heart.</p>
        </footer>
    </div>

    <script>
        function toggleCheck(element) {
            const checkbox = element.querySelector('input[type="checkbox"]');
            checkbox.checked = !checkbox.checked;
            element.classList.toggle('checked', checkbox.checked);
            saveCheckState();
        }

        function clearAllChecks(pageId) {
            const page = document.getElementById(pageId);
            const checkboxes = page.querySelectorAll('input[type="checkbox"]');
            checkboxes.forEach(cb => {
                cb.checked = false;
                cb.closest('.grocery-item').classList.remove('checked');
            });
            saveCheckState();
        }

        function saveCheckState() {
            const allCheckboxes = document.querySelectorAll('.grocery-item input[type="checkbox"]');
            const checkState = {};
            allCheckboxes.forEach((cb, index) => {
                checkState[index] = cb.checked;
            });
            localStorage.setItem('groceryChecks', JSON.stringify(checkState));
        }

        function loadCheckState() {
            const saved = localStorage.getItem('groceryChecks');
            if (saved) {
                const checkState = JSON.parse(saved);
                const allCheckboxes = document.querySelectorAll('.grocery-item input[type="checkbox"]');
                allCheckboxes.forEach((cb, index) => {
                    if (checkState[index]) {
                        cb.checked = true;
                        cb.closest('.grocery-item').classList.add('checked');
                    }
                });
            }
        }

        function changePage() {
            // Hide all pages
            const pages = document.querySelectorAll('.page');
            pages.forEach(page => page.classList.remove('active'));
            
            // Show selected page
            const selector = document.getElementById('pageSelector');
            const selectedPage = document.getElementById(selector.value);
            if (selectedPage) {
                selectedPage.classList.add('active');
                window.scrollTo({ top: 0, behavior: 'smooth' });
            }
        }

        // Initialize
        window.onload = function() {
            changePage();
            loadCheckState();
        };
    </script>
</body>
</html>Weekend Flexibility:</strong> Mix and match any leftover proteins with salads and pita for easy lunches and dinners.
                </div>
            </div>

            <!-- WEEK 2 GROCERY -->
            <div id="week2-grocery" class="page">
                <h2>Week 2: Tex-Mex Favorites</h2>
                <h3>Grocery List</h3>

                <div class="grocery-list">
                    <div class="grocery-category">
                        <h4>Proteins:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lb ground beef (90% lean or leaner) or ground turkey</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lb boneless skinless chicken thighs</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 can black beans (no salt added or low sodium)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 can pinto beans (no salt added or low sodium)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Shredded cheese (reduced-fat cheddar)</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Vegetables:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>2 bell peppers (red and green)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>3 tomatoes</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 large onion</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 bag baby spinach</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 avocado</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>1 lime</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Jalapeño (optional)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Cilantro (fresh)</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Pantry & Staples:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Corn tortillas (small, whole grain)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Brown rice</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Salsa (jar, low sodium)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Low-sodium taco seasoning</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Extra virgin olive oil or cooking spray</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Garlic powder</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Cumin</label>
                            </li>
                        </ul>
                    </div>

                    <div class="grocery-category">
                        <h4>Extras:</h4>
                        <ul>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Plain non-fat Greek yogurt (for sour cream substitute)</label>
                            </li>
                            <li class="grocery-item" onclick="toggleCheck(this)">
                                <input type="checkbox" onclick="event.stopPropagation()">
                                <label>Hot sauce (optional)</label>
                            </li>
                        </ul>
                    </div>
                    
                    <button class="clear-checks-btn" onclick="clearAllChecks('week2-grocery')">Clear All Checks</button>
                </div>
            </div>

            <!-- WEEK 2 MEALS -->
            <div id="week2-meals" class="page">
                <h2>Week 2: Tex-Mex Favorites</h2>
                <h3>Daily Meals</h3>

                <div class="meal-card">
                    <h4>Monday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Black bean and rice bowl</strong></p>
                    <div class="cook-extra">
                        🍚 COOK EXTRA RICE TODAY - Make 2 cups dry rice for the week
                    </div>
                    <div class="meal-instructions">
                        <em>How to make:</em> Reheat 1 cup cooked brown rice. Top with ½ can drained black beans (warmed), 1 diced tomato, 2 tablespoons salsa, 2 tablespoons shredded cheese. Add hot sauce if you like heat!
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Ground beef tacos with peppers and onions</strong></p>
                    <div class="cook-extra">
                        🥩 COOK THE FULL POUND - You'll use half tonight and save the rest
                    </div>
                    <div class="meal-instructions">
                        <em>How to make:</em> Brown 1 lb ground beef in a large skillet over medium-high heat, 7-8 minutes. Drain any excess fat. Add 1 packet taco seasoning (or DIY: 1 tablespoon chili powder, 1 teaspoon cumin, ½ teaspoon garlic powder, salt). Add ½ cup water, simmer 5 minutes.<br><br>
                        Meanwhile, sauté 1 sliced bell pepper and ½ sliced onion in 1 teaspoon olive oil until tender, about 8 minutes.<br><br>
                        <em>Eat tonight:</em> Use half the taco meat. Warm 3-4 corn tortillas. Fill with meat, peppers, onions, salad greens, and a dollop of Greek yogurt.
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Tuesday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Taco salad with beans and salsa dressing</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Arrange 2 cups spinach on a plate. Top with ⅓ cup reheated taco meat, remaining black beans, 1 diced tomato, and 2 tablespoons salsa as dressing. Add a squeeze of lime if you have it.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Grilled chicken thighs with peppers and pinto beans</strong></p>
                    <div class="cook-extra">
                        🍗 COOK ALL 4 THIGHS - Save extras for later this week
                    </div>
                    <div class="meal-instructions">
                        <em>How to make:</em> Season 1 lb chicken thighs with olive oil, cumin, garlic powder, salt and pepper. Grill or bake at 400°F for 25-30 minutes until internal temp reaches 165°F.<br><br>
                        Sauté remaining bell pepper and onion half in 1 tablespoon olive oil, 8-10 minutes.<br><br>
                        Warm ½ can pinto beans on the stove with a pinch of cumin.<br><br>
                        <em>Eat tonight:</em> 2 chicken thighs with half the vegetables and beans.
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Wednesday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Bean and veggie burrito bowl</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Build your bowl with 1 cup reheated rice, remaining pinto beans (warmed), leftover sautéed peppers and onions, 3 tablespoons salsa, 2 tablespoons cheese. Top with cilantro if you have it.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Chicken fajitas with corn tortillas</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Slice 1 leftover chicken thigh into strips. Sauté in a pan with any remaining peppers/onions (or slice a fresh one), 1 teaspoon extra virgin olive oil, cumin, and chili powder, 5-7 minutes.<br><br>
                        Warm 3-4 corn tortillas. Serve chicken and veggies with tortillas, salsa, and non-fat Greek yogurt.
                    </div>
                    <div class="flavor-tip">
                        <strong>Flavor twist:</strong> Add a squeeze of lime and fresh cilantro for brighter flavor!
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Thursday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Chicken and spinach salad with avocado</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Slice remaining chicken thigh. Arrange 2 cups spinach, add chicken, any leftover beans, 1 diced tomato, ½ sliced avocado. Squeeze lime over everything, drizzle with 1 tablespoon extra virgin olive oil, sprinkle with salt and pepper.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Beef and bean skillet over rice</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Reheat remaining taco meat in a skillet. Add 1 diced tomato, any leftover beans, ½ teaspoon cumin, pinch of chili powder. Stir and cook 5 minutes until heated through.<br><br>
                        Serve over 1 cup reheated rice. Top with cheese and salsa if desired.
                    </div>
                </div>

                <div class="meal-card">
                    <h4>Friday</h4>
                    
                    <p><span class="meal-label">LUNCH</span> <strong>Quesadilla with chicken or beans</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Heat a skillet over medium heat. Place 1 corn tortilla in pan, sprinkle with 3 tablespoons cheese, add any leftover chicken (shredded) or beans, top with another tortilla. Cook 2-3 minutes per side until golden and cheese melts. Cut into wedges. Serve with salsa.
                    </div>

                    <p style="margin-top: 20px;"><span class="meal-label">DINNER</span> <strong>Mexican-style scrambled eggs</strong></p>
                    <div class="meal-instructions">
                        <em>How to make:</em> Scramble 3 eggs in 1 teaspoon olive oil. Add any remaining peppers/onions, a few tablespoons of beans, cook until eggs are set. Top with salsa and cheese.<br><br>
                        Serve with warm corn tortillas on the side.
                    </div>
                </div>

                <div class="tip-box">
                    <strong>
