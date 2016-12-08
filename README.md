
当一些展示页面的lable即使缩小字体也不能完全放下需要展示的字符的时候，或者需要一些广告/公告信息的时候可以考虑下跑马灯效果(本文结合一些网络资源,进行一些需求的综合)提供的一些属性如下：

		
	/**
	 内容文字（富文本存在时以富文本为准text的常规设置失效）
	 */
	@property (nonatomic, strong) NSString *text;

	/**
	 字体 默认15
	 */
	@property (nonatomic, strong) UIFont *font;

	/**
	字体颜色
	 */
	@property (nonatomic, strong) UIColor *textColor;

	/**
	富文本（富文本存在时以富文本为准text的常规设置失效）
	 */
	@property (nonatomic, strong) NSAttributedString *attributedText;
	
	/**
	 速度
	 */
	@property (nonatomic, assign) NSInteger speed;
	
	/**
	循环滚动次数(为0时无限滚动)
	 */
	@property (nonatomic, assign) NSUInteger repeatCount;

	/**
	 第二遍开始与第一遍结束之间的空格大小
	*/
	@property (nonatomic, assign) CGFloat leastInnerGap;

	/**
	 是否结束停留
	 */
	@property(nonatomic,assign)BOOL IsEndStay;

	/**
	 重载
	 */
	- (void)reloadView;
